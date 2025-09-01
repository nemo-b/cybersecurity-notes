# 🛡️ Cybersecurity Tools: Core Tools & Skills to Learn

The goal of this section is to take basic notes on my learning adventure — documenting what I explore, practice, and understand over time. With some basic research, I learned that these are generally the most used tools for cybersecurity, so I hope this can become applicable knowledge later down the line.  

---
## 📂 Tools Index
- [x] 1. **Wireshark** (Completed: Aug 25, 2025)
- [ ] 2. **Splunk** (In Progress)
- [ ] 3. **Nmap**
- [ ] 4. **Metasploit Framework**
- [ ] 5. **Burp Suite**
- [ ] 6. **Kali Linux Tools (General)**
- [ ] 7. **Security Onion**
- [ ] 8. **Snort / Suricata (IDS/IPS)**
- [ ] 9. **VMs & Sandbox Environments**
- [ ] 10. **Python for Cybersecurity**
- [ ] 11. **Volatility (Memory Forensics)**
- [ ] 12. **GRC Tools (Governance, Risk, Compliance)**

---

## 🔬 Lab Notes Format (for each tool)

### 🧰 Tool: Wireshark ✅
*Completed: Aug 20, 2025*

**Purpose / Role:**  
WireShark is a network protocol analyzer that lets you capture and inspect packets traveling across a network. Its essential for network troubleshooting, detecting suspicious traffic, and understanding protocols at a deep level. 

**Core Skills to Learn (according to ChatGPT):**  
- [x] Install / Setup  
- [x] Basic Commands  
- [x] Common Use-Cases  
- [x] Using it on my network  

## Notes:
To learn Wireshark, I started with **YouTube tutorials**, and whenever I didn’t understand something I had just seen (or had a question the video didn’t answer), I asked ChatGPT for clarification.

**First video I used to learn is this:**  
[Learn Wireshark in 10 minutes - Wireshark Tutorial for Beginners - Vinsloev Academy](https://www.youtube.com/watch?v=lb1Dw0elw0Q&t=68s)

The video began with download instructions, but since I’m on Linux, I was able to quickly find Wireshark in the app center.

The first noticeable detail was the short list of different networks connected to my machine. Each one had small, updating graphs showing how much traffic was moving through that connection. One key point (at least for me) was that if I want to track things like _who is visiting which sites on my network_, I could connect via **Ethernet cable** to my router and track the Ethernet interface directly. Public Wi-Fi networks are generally encrypted from methods like this (as the video explained). Also, as a security best practice: never connect to open public Wi-Fi.

To start watching a network, you simply double-click one of the available interfaces. On my laptop, I tested this using `wlp1s0`. After connecting to an active network, I started seeing many packets (logs). They are clearly categorized at the top with columns like **No., Time, Source, Destination, Protocol…**. For my initial testing, I focused on the **Protocol** column.

This is where the video introduced filtering (though I had already started experimenting with this myself). At the top of the window there’s a filter bar: if you type in, for example, `http`, Wireshark only shows HTTP packets. Since HTTP is insecure, I didn’t see much of it on my machine, but I did find useful packets under protocols like **DNS**.

After I started seeing results, I wanted to understand how to “translate” what was on my screen — so I asked ChatGPT.

#### Default Wireshark Columns
- **No. (Number)** → The order the packet was captured in
- **Time** → A timestamp of when the packet was seen
- **Source** → The sender’s address (IP, MAC, or hostname, depending on the layer)
- **Destination** → The receiver’s address
- **Protocol** → What “language” they’re speaking (TCP, UDP, HTTP, DNS, TLS…)
- **Length** → The size of the packet
- **Info** → A quick summary of what’s inside the packet

#### Filtering Issues
One thing I found interesting — but couldn’t get working — was detailed filtering, specifically using `tcp contains youtube`. After troubleshooting with ChatGPT, I learned that the problem was encryption: since YouTube uses HTTPS, the word “youtube” doesn’t appear inside the packet contents. Instead, you need to look at **metadata** around the connection.

The most useful solution for me was:

`dns.qry.name contains "youtube"`

This worked perfectly!

#### ChatGPT’s Suggested Alternatives

> 1. **Use DNS Queries (best method for domains)**
>     
>     - Filter: `dns.qry.name contains "youtube"`
>         
>     - Shows when a device asks a DNS server to resolve `youtube.com`.
>         
> 2. **Look at SNI (Server Name Indication) in TLS Handshake**
>     
>     - Filter: `tls.handshake.extensions_server_name contains "youtube"`
>         
>     - Works unless TLS 1.3 + ESNI hides it.
>         
> 3. **Filter by IP Ranges**
>     
>     - Example: `ip.addr == 142.250.0.0/15` (Google’s IP range).
>         
> 4. **Quick Check**
>     
>     - Use the simple `dns` filter to see every site your device asked for.
>         

#### Packet Bytes Pane
While tinkering, I noticed another section in Wireshark — the raw data at the bottom of the screen. When I hovered over different parts, the left box highlighted the related section in plain English.

Later, I learned from ChatGPT that this section is called the **Packet Bytes Pane**. The right-side box was essentially a _translation_ of the raw packet data into something more human-readable.

This connects back to the video: when the instructor searched for `tcp contains youtube`, Wireshark was actually looking for the word “youtube” inside this **packet bytes** section.

#### The Three Panes in Wireshark
1. **Top Pane (Packet List Pane)**
    - Each row = one packet
    - Shows No., Time, Source, Destination, Protocol, Info
2. **Middle Pane (Packet Details Pane)**
    - Expands the packet into protocol fields (Ethernet, IP, TCP, HTTP, etc.)
    - Like a “translation guide” of the raw bytes
3. **Bottom Pane (Packet Bytes Pane)**
    - Shows the raw data as captured
    - **Left side** → Byte offset (positions in the packet)
    - **Middle column** → Hexadecimal values (actual bytes)
    - **Right column** → ASCII representation (human-readable characters, when possible)

#### Plaintext Traffic Example
The video also showed an example of capturing **unencrypted data**. The instructor visited a test site that used **HTTP** instead of HTTPS. He entered a login (`admin123`) on the site, and then used the filter:

`tcp contains admin123`

Sure enough, the username appeared in plaintext in the packets. This is a clear example of why HTTP is insecure — anyone capturing traffic could read the username or even the password.

##### Key Takeaways
- Learned how to filter packets generally.
- Surprised by how much “background noise” is always on a home network.
- Still need to revisit details of different protocols (this part is confusing for me).
