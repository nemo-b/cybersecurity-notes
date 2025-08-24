**The Basics of Computing Security: Linux & SQL**

COURSE LEARNINGS:

- Operating systems and how they relate to applications and hardware
- The Linux operating system
- The Linux operating system
- SQL to query databases

**Hardware**: The physical components of a computer

**Application**: A program that preforms a specific task

**User interface (UI)**: A program that allows the user to control the functions of the operating system

**Graphical user interface (GUI)**: A user interface that uses icons on the screen to manage different tasks on the computer

**Basic GUI components**

- Start menu
- Task bar
- Desktop with icons and shortcuts

**Command line interface (CLI)**: A text based user interface that uses commands to interact with the computer

**Linux**: An open-source operating system

**Open-source**: Open-source refers to a type of software that is freely available for the public to use, modify, and distribute. It allows users to access and modify the source code of the software, promoting transparency and collaboration among developers.

In the context of computing security, open-source software can provide advantages such as increased security through community scrutiny and the ability to customize and audit the code for potential vulnerabilities.

**Components of Linux:**

- **User** - The person interacting with a computer.
- **Applications** - A program that runs a specific task.
- **Shell** - The command-line interpreter (how you communicate with the system).
- **Filesystem Hierarchy Standard** (FHS)- The component of the Linux OS that organizes data.
- **Kernel** - The component of the Linux OS that manages processes and memory.
- **Hardware** - The physical components of a computer.

**Distributions**: The different versions of Linux (also known as “distros” or “flavors of Linux”) 

Parent Distributions:

- Red hat (CentOS)
- Slackware (SUSE)
- Debian (Ubuntu and KALI LINUX)

Digital forensics tools in KALI LINUX

- tcpdump
- Wireshark
- Autopsy

**Command**: An instruction telling the computer to do something

**Standard input**: Information received by the OS via the command line

**echo**: A Linux command that outputs a specified string of text

- EX: nemonatie@Abels-iMac-2 ~ % echo hello

**String data**: Data consisting of an ordered sequence of characters

**Standard error**: Error messages returned by the OS through the shell

- EX: nemonatie@Abels-iMac-2 ~ % eco hello

**Bash**: The default shell in most Linux Distributions

**Argument (Linux)**: Specific information needed by a command

**Root directory**: The highest-level directory in Linux

**pwd**: Prints the working directory onto the screen

**ls**: Displays the names of files and directories in the current working directory

**cd**: Change directories

**cat**: Displays the content of a file

**head**: Displays just the beginning of a file, by default 10 lines

**grep**: Searches a specified file and returns all lines in the file containing a specified string

- EX: grep Lorem Lorem_ipsum.txt

![Screen Shot 2024-01-01 at 11.47.52 AM.png](Screen_Shot_2024-01-01_at_11.47.52_AM.png)

![Screen Shot 2024-01-01 at 11.56.46 AM.png](Screen_Shot_2024-01-01_at_11.56.46_AM.png)

**Piping**: Sends the standard output of one command as standard input to another command for further processing

To look for directories that only contain a specific word. You would put something like this “**ls /home/analyst/reports | grep users**”, ****this is just an example**.**

**mkdir**: Creates a new directory

**rmdir**: Removes, or deletes, a directory

**touch**: Creates a new file

**rm**: Removes, or deletes, a file

**mv**: Moves a file or directory to a new location

**cp**: Copies a file or directory into a new location

Permissions in Linux

- Read
- Write
- Execute

Types of owners

- User (First rwx) = u
- Group (Second rwx) = g
- Other (Third rwx) = o

Example of full permission: (d)(rwx)(rwx)(rwx), the “rwx” shows what permissions a certain owner group has

**Options**: Modify the behaviors of the command

**ls -l**: Displays permissions to files and directories

**ls -a**: Displays hidden files

ls -la: Displays permissions to files and directories, including hidden files (A combination of the two aforementioned)

chmod: Changes permissions on files and directories; change mode

- EX: chmod g+w, o-r access.txt

**Root user (or superuser)**: A user with elevated privileges to modify the system

**Problems with logging in as root**

- Security risks
- Irreversible mistakes
- Accountability

**sudo**: Temporarily grants elevated permissions to specific users

**useradd**: Adds a user to the system

**userdel**: Deletes a user from the system

for the userdel and useradd you know the progress was completed successfully when another dash comes up and not an error message. Also, you should start the code with “sudo”, here is an example.

- EX: sudo userdel salesrep7

**man**: Displays information on other commands and how they work (manual)

**Primary key**: A column where every row has a unique entry

**Foreign key**: A column in a table that is a primary key in another table

**SQL (Structured Query Language)**: A programming language used to create, interact with, and request information from a database

**Query**: A request for data from a database table or a combination of tables

**Log**: A record of events that occur within an organization’s systems

**SELECT**: Indicates which columns to return

**FROM**: indicates which table to query

**Syntax**: The rules that determine what is correctly structured in a computing language

**Filtering**: Selecting data that match a certain condition

**Operator**: A symbol or keyword that represents an operation

- EX: country = ‘USA’

**WHERE**: Indicates the condition for a filter

- EX: WHERE country = ‘USA’

![Proper usage of the SQL commands above](Screen_Shot_2024-01-02_at_9.08.04_PM.png)

Proper usage of the SQL commands above

**LIKE**: Used with ”WHERE” to search for a pattern in a column

**Numeric data**: Data consisting of numbers

**Date and time data**: Data representing a date and/or time

**Operators**:

- = (Equal to)
- > (Greater than)
- < (Less than)
- <> (Not equal to)
- >= (Greater than or equal to)
- <= (Less than or equal to)

BETWEEN: An operator that filters for numbers or dates within a range

**AND**: Specifies that both conditions must be meet simultaneously

**NOT**: Negates a condition

**INNER JOIN**: Returns rows matching on a specified column that exists in more than one table

**LEFT JOIN**: Returns all of the records of the first table, but only returns rows of the second table that match a specified column

RIGHT JOIN: Returns all of the records of the second table, but only returns rows from the first table that match on a specified column

FULL OUTER JOIN: Returns all records from both tables