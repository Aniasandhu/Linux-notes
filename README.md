# Linux notes
<<<<<<< HEAD
=======
+-----------------------------------------+
| cybersecurity notes                               |
| Ania                                    |
+-----------------------------------------+


Navigation in Linux
-------------------

Commands List:
- ls
- cd
- pwd
- mkdir
- rmdir

Command Details:
----------------

- `ls`
  - Purpose: Lists the contents of a directory.
  - Usage: `ls` for basic listing, `ls -l` for detailed listing, `ls -a` to include hidden files.
  - Notes: Essential for quickly viewing what's in the current directory.

- `cd`
  - Purpose: Changes the current directory.
  - Usage: `cd [directory path]` to move to a specific directory, `cd ..` to move up one directory level, `cd` or `cd ~` to return to the home directory.
  - Notes: Most commonly used for navigating through the filesystem.

  'Cp'
  Purpose: copy files and directory
  Usage: 'cp file.txt /newfolder/' copies file to /newfolder/.

- `pwd`
  - Purpose: Prints the current directory path.
  - Usage: `pwd` to display the full path of the current directory.
  - Notes: Useful for confirming your current location in the filesystem.

- `mkdir`
  - Purpose: Creates a new directory.
  - Usage: `mkdir [directory name]` to create a new directory in the current location.
  - Notes: Handy for organizing files into new folders.

- `rmdir`
  - Purpose: Removes a directory.
  - Usage: `rmdir [directory name]` to delete an empty directory.
  - Notes: Used for cleaning up and removing unused directories. Note that the directory must be empty.

  cat filename.txt — Displays the contents of a file.

less filename.txt — Allows you to scroll through a file.
-To leave is Ctrl z

echo "Text" &gt;&gt; filename.txt — Appends text to a file.

Permissions are shown as -rwxrwxrwx, divided into User (u), Group (g), and Others (o).
r — Read (4)
w — Write (2)
x — Execute (1)

-chmod u+x filename — Adds execute permission for the user.
-chmod g-w filename — Removes write permission from the group.
-chmod 755 filename — Sets permissions to rwxr-xr-x.
ls -l-To view permissions.

sudo [command] — Runs a command with superuser privileges.
Example: sudo apt update — Updates package lists.
sudo su - get into root user
-sudo nano /root/filename.txt-To create file
-sudo ls /root

cd / -To get into root directory 
-USe sudo before command 
Example: sudo touch filename.txt
cd ~ to get back

Type man [command] in the terminal for the manual.

Make folder: mkdir foldername 

Make files: touch filename.txt 

Put writing int file: echo “message”> filename.txt 

Move files into folders: mv filename.txt foldername/ 

Edit message in file: nano filename.txt 

-Nano opens 

-Rewrite message 

-CTRL+o 

-Enter 

-CTRL+x 

Delete files (inside folder/outside folder): rm filename.txt 

Delete folders: rmdir ./foldername/ 

 1.IP address 

A unique address that identifies a device on the internet or a local network. IP stands for “Internet Protocol,” which is the set of rules governing the format of data sent via the internet or local network.  

2. Subnet Masks 

A 32-bit number that divides an IP address into network and host portions, enabling efficient addressing. It is used to identify the network and host parts of an address. 

 3. Gateway 

A gateway can refer to a point of access to information, services, or resources. For example, a website or portal that provides access to various online services can be called a gateway. 

 4. DNS 

It is a hierarchical and decentralized system that translates human-readable domain names into numerical IP addresses, which are used by computers to identify each other on a network. 

5. What is a network switch 

A network switch is a networking device that operates at data link layer of the OSI (Open System interconnection) 

 6. What is a network router 

A network router is a device that connects different networks together, directing data traffic between them. 

7. What are “access points” 

An access point (AP) is a device that allows wireless devices, such as computers, smartphones, or tablets, to connect to a wired network using Wi-Fi (wireless) communication. 

8. Mac address 

A MAC address, or Media Access Control address, is a unique identifier assigned to network interfaces for communications at the data link layer of a network. 

 9. What are “ports” in networking addressing  

In networking, ports are like virtual endpoints for communication. They allow a computer to distinguish between different services or processes running on it. 

10. Types of networks (WAN, LAN, PAN, MAN, and VPN) 

 **Types of Networks:** 

    - **WAN (Wide Area Network):** A network that spans a large geographical area, connecting multiple LANs. 

    - **LAN (Local Area Network):** A network that is limited to a small geographic area, such as a single building or campus. 

    - **PAN (Personal Area Network):** A network for personal devices, typically within the range of an individual person, such as Bluetooth connections. 

    - **MAN (Metropolitan Area Network):** A network that covers a larger geographic area than a LAN but is smaller than a WAN, usually within a city. 

    - **VPN (Virtual Private Network):** A secure network connection over the Internet that allows users to access private networks remotely. 


**Exploring Commands:** 

1. **ifconfig:** Displays information about network interfaces on a system, including IP addresses, MAC addresses, and interface status.  

2. **ip:** A versatile command for configuring and displaying network interfaces, IP addresses, routes, and more.  

3. **traceroute:** Traces the route that packets take to reach a destination, showing each hop along the way.  

4. **tracepath:** Similar to traceroute, it provides the route taken by packets to a destination.  

5. **ping:** Sends ICMP Echo Request messages to a specified network host to test the reachability of the host and measure the round-trip time for messages to travel from the source to the destination.  

6. **netstat:** Displays network statistics, including open ports and active connections.  

7. **ss:** Another tool for displaying information about sockets and network connections.  

8. **dig:** Queries DNS name servers for DNS information, such as domain name details, IP addresses, and related information.  

9. **nslookup:** A tool for querying DNS servers to obtain domain name or IP address mapping information.  

10. **route:** Displays or modifies the IP routing table. 

 11. **host:** A DNS lookup utility to find the IP address of a domain or the domain associated with an IP address.  

12. **arp:** Displays and modifies the ARP cache, which maps IP addresses to MAC addresses. 

 13. **iwconfig:** Configures wireless network interfaces.  

14. **hostname:** Displays or sets the hostname of a system.  

15. **curl or wget:** Commands for downloading files from the internet.  

16. **mtr:** Combines the functionality of ping and traceroute to provide a continuous stream of information about the network path between two hosts.  

17. **whois:** Retrieves information about the registered users of an Internet resource, such as a domain name or IP address.  

18. **ifplugstatus:** Checks the status of plugged-in network cables.  

19. **iftop:** Displays a list of network connections in real-time, showing data rates and data traffic.  

20. **tcpdump:** Captures and analyzes network traffic. 

Git:

•Initialize Repository:
bash - [git init]
• Configure Git:
bash - [git config --global user.name "Your Name"]
bash - [git config --global user.email "youremail@example.com"]
• Check Status:
bash - [git status]
• Stage Files:
bash - [git add filename]
bash - [git add .]
• Commit Changes:
bash - [git commit -m "message"]
• View Log:
bash - [git log]
• Create and Switch Branch:
bash - [git checkout -b branch-name]
• Switch Branch:
bash - [git checkout branch-name]
• Merge Branches:
bash - [git merge branch-name]
• Delete Branch:
bash - [git branch -d branch-name]
• Undo Changes in Working Directory:
o Using git restore (newer versions):
bash - [git restore filename]
o Using git checkout (older versions):
bash - [git checkout -- filename]
• Remove Cached File:
bash - [git rm --cached filename]
• Set Alias:
bash - [git config --global alias.alias-name command]
• Tag a Commit:
bash - [git tag -a v1.0 -m "message"]
• Reset Commits:
bash - [git reset --soft HEAD~1]
bash - [git reset --hard HEAD~1]
>>>>>>> 5f7d605 (Initial commit)
