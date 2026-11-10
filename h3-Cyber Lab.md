# X) Read and summarize  

**How to install Linux to VirtualBox**  
- The article is about installing Linux to a virtual box, it initially explains how to install Oracle VirtualBox on Windows 11.
- The prerequisite to install virtual machine is to enable VT-X in machine’s BIOS setting.
- It introduces Debian Linux and different Linux distributions. It then explains downloading the Debian ISO file.
- Explains creating a virtual machine and allocating RAM, CPU and disk space.
- It also introduces BIOS, UEFI and Secure Boot.
- Demonstrates testing Debian using Live Install before installation.
- Covers Debian installation, including language, keyboard and disk partitioning.
- Explains updating the system using apt-get update and apt-get upgrade.

**Command Line Basics Revisited**  
- The article introduces basic Linux terminal commands for navigating folders and checking files.
- Explains how to create, copy, move, rename and delete files and directories.
- Shows how to read files and get help using commands like less, man and --help.
- Introduces SSH for connecting to remote computers and SCP for transferring files.
- Explains useful shortcuts such as Tab for auto-completion and arrow keys to repeat commands.
- Mentions important Linux directories and their purposes.
- Explains how to use sudo for administrative tasks.
- Introduces package management commands for installing and updating software.

**Cracking Passwords with Hashcat**  	
- The article explains that passwords are usually stored as hashes rather than plain text. Hashing makes it difficult to get the original password back directly.
- Introduces Hashcat  tool that helps test different passwords to see if they match a given hash.
- Shows how to install Hashcat and the necessary tools on Linux.
- Explains how to download and use the RockYou password list, which contains millions of commonly used and previously leaked passwords.
- Shows how to identify the type of hash using hashid before starting the cracking process.
- Demonstrates a dictionary attack using Hashcat, where the password is successfully discovered.
- Explains how to view and save the recovered passwords. It also mentions that using a GPU can make the process much faster.

# a)	Reserve presentation title in Laksu  
Reserved in Laksu.  
Title: From Hacked Fridges to Secure Smart Homes: An IoT Maturity Perspective


# b)	Linux Installation

- Installed Oracle Virtualbox from the link provided in the article https://github.com/johannaheinonen/johanna-test-repo/blob/main/module_1.md
- Downloaded debian iso image from the link provided in the article. I chose debian 13.7.0 cinnamon  
 https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/
- Followed the article to set up new virtual machine and start the newly installed machine.
- Installed the debian using installer as mentioned in the article.
- Updated the package list as mentioned in the article.

# c)	Crack the hash

- Installed hashcat on debian vm  
$ sudo apt-get update  
$ sudo apt-get –y install hashid hashcat wget  

- To identify hash type I used the following command  
$ hashid 6b1628b016dff46e6fa35684be6acc96  

- For dictionary, I used RockYou using following command  
$ wget https://github.com/danielmiessler/SecLists/raw/master/Passwords/Leaked-Databases/rockyou.txt.tar.gz  
$ tar xf rockyou.txt.tar.gz  
$ rm rockyou.txt.tar.gz  
  
- Then I used following hashcat command to recover the password  
$ hashcat -m 0 6b1628b016dff46e6fa35684be6acc96 rockyou.txt  
  
- The password is “summer”



