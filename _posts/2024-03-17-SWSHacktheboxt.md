---
Title: SWS Cyber Security
categories: [SWS, Hack the box]
tags: [Tier 0 , TIer 1]
---

### Topic :Hack the box Tier 0 to 1

Tier 0(meow)

this tier starts with first connecting it into HTB(hack the box ) server or openvpn so that we can spawn the machine or to start the machine.

To connect to openvpn we must download the starting point of the file of the open vpn and the run the the code "sudo openvpn "file name"" which will connect us in the vpn.

Task 1

The answer to task 1 is virtual machine as the word virtual machine can be virtual system running in our pc to replicate the work of pc but in differnt way or a virtual machine is a computer file, typically called an image, that behaves like an actual computer. It can run in a window as a separate computing environment, often to run a different operating system—or even to function as the user's entire computer experience—as is common on many people's work computers.

Task 2

The tool we use to interact with the operating system in order to issue commands via the command line, such as the one to start our VPN connection is Terminal where the terminal .

Task 3

The svervice of vpn connection used in HTB labs is opnevpn.

Task 4

The answer is ping as the t sends Internet Control Message Protocol (ICMP) Echo Request messages to a target host (the device being tested) and waits for a response.
the code in the terminal to scan can be run as "ping "our ip address""

Task 5

The answer is Nmap as Nmap (“Network Mapper”) is an open source tool for network exploration and security auditing. It was designed to rapidly scan large networks, although it works fine against single hosts.

Task 6

The answer is telnet which is a protocol that provides a command line interface for communication with a remote device or server and the way got the answer is telnet is because when i use the code for nmap to run all ports to do service nuemeration where the code goes as "nmap -p- sV "ip address"" and when i run this to run all port i can see under the output port 23 or porr state vesion 23/tcp open telnet.

task 7

The answer is root as first we have to connect to the hack the box in the terminal by using the code "tlenet "ip address"" which will login us to HTB server and then we are asked for username and the username is root which will process needs privileged access to run where a standard user is non-privileged. This means an account that isn't able to make changes to the OS. The equivalent in Windows is the Administrator.

task 8

For task 8 the process is continution to task 8 as after i get access as root user and login, i am not privilledged as root user which have highest acces so i can simply use code "ls" to list the file and it gives me file "flag.txt" and to get the root flag its just like the one we did in bandit over the wire as the code goes "cat flag.txt" which gives us the output for the password or rootflag.

TIER 0(Fawn)

Task 1
FTP stands for file transfer prtocol which means  standard network protocol used for the transfer of files from one host to another over a TCP-based network, such as the Internet. FTP works by opening two connections that link the computers trying to communicate with each other.

Task 2

The answer is 21 or Port 21 as Port 21 is used for pass control information. And the other port 20 is used to send the data files between the client and the server. FTP ports 20 and 21 must both be open for successful file transfer on the network

Task 3

The answer is SFTP which is known as  network protocol for securely accessing, transferring and managing large files and sensitive data.

task 4

The answer is ping  

Task 5

The anwer is "vsftpd 3.0.3" as when we use nmap to scan the ip addresss using the code "nmap -sV " which gives us the output
 "PORT   STATE SERVICE VERSION
21/tcp open  ftp     vsftpd 3.0.3"
we can see the ftp version .

Task 6

The answer is Unix as it is same step like Task 5 using code "nmap -sV " we get the output 
Service Info: OS: Unix
So we can learn that OS type is Unix.
Unix allows each user to run more than one job at a time allowing for a switch of attention between jobs. This multitasking ability allows users to be more productive. The X Window System makes it easier to keep track of all your different processes by allowing multiple viewports to your work environment.

Task 7

The answer is ftp -h as it gives us helping information on FTP.

Task 8

The answer is anoymous as it meands that it is not identified as we use the code to enter into the server ftp -v "ip address" we get to enter a username which we can put anoymous as it means undefined.

Task 9

The answer is 230 as it goes continution to task 8 as we put the username anoymous we get to enter password which we dont know so we use nothing written in password because server responds with 230 status as it means the server lets us procced with te username and password.

Task 10

The answer is ls for list

Task 11

The answer is get.

Task 12

To get the root flag we procced with task 8 after entering the password with nothing typing we use the command ls which gives us list of file so we use the command to download file on ftp server by using the code "get flag.txt " so we get the root flag.

Tier 0 (redemmer)

Task 1

the answer is port 6379 as we can get the TCP by using nmap scan with port with the code "nmap -p- --min-rate 5000 -sV 10.129.183.243" so we get the TCP.

task 2
the asnwer is reids and it is same like task 1 as it is nmap scanning and we get the output where it shows that service is running on port redis.

Task 3

The answer is in-memory Database as a purpose-built database that relies primarily on internal memory for data storage. 

Task 4

the answer is redis-cli but we have to install redis tool to run this code .

Task 5

the answer is -h this program is called redis-cli. Running redis-cli followed by a command name and its arguments will send this command to the Redis instance running on localhost at port 6379.

Task 6

to connect to to redis server we have to use the code "redis-cli -h "ip address"" which connects us to redis server and to obtain information we use the code info which gives all the details of info

Taks 7

after using the code info we can see the information of the server where it shows server 5.0.7    .

Task 8

the command used is select.

Task 9

so we use the comand "select 0" which selects the database with index 0 and then we use command "keys *" to help us show the keys of the selected to database.

Task 10

To get to root flag we use the command "get" and we know the flag file is in the database so we use command get flag which gives us the root flag.

Tier 1()