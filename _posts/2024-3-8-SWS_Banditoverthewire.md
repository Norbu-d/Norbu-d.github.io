---
Title: SWS Cyber Security
categories: [SWS, bandit over the wire]
tags: [SWS]
---

### Topic : Bandit Over the wire level 0 -> 20

## level 0

echo bandit0 > 0;sshpass -p$(cat 0) ssh bandit0@bandit.labs.overthewire.org -p 2220
this code creates a file called 0 which stroes every password for everylevel for different lelvel .
this code use command substitution where "cat 0" gives us output bandit 0 which will be supplied by "-p" which stands for
 password in ssh passs and then we are telling ssh to connect to this partiucularhost "bandit0@bandit.labs.overthewire.org "
 with username bandit 0 and pasword 2220

## level 0 -> 1

in this level the pasword is stored in readme file where readme file can be found using the code "ls" which gives us the
 list of file and we get the file read me and to get the pasword we use a code called "cat readme" or "cat filename"
 as  his command is short for "concatenate" and is often used to display the contents of one or more files to the terminal.
 
## level 1 -> 2

the password in this level is in - which speacial charater key and as like level 0 to "cat -" cannot work as it is a special 
charater key so we use the code "cat ./-"ttempts to display the contents of a file named "-" in the current directory \
using the cat command.

## level 2 -> 3

in this level the pasword is stored in a file called space in this filename.
we first use the code "ls" which gives us space in the filename and after using code "ls -la" we can see that it is one file 
whcih has differnt spaces so if we use the "cat space in the filename" it will give us error as it reads it individually for 
space , in , the , filename differntly so we get error and to solve this problem we use code "cat spaces\ in\ the\ filename"
called escape sequence so that we can read the file altogether instead of reading it individually as it doesnnot get divided.

## level 3 -> 4

in this level the password is hidden in the file called inhere directory.
we have to use the code "ls" which gives us the list of file so we "in here " file to get into the file we use a code called
"cd inhere/" which gives us acces to the file and to find the pasword we use "ls-la" but it gives us lots of file so we use 
another code called "ls -a" used to list all files and directories in the current directory, including hidden files and directories.

## level 4 -> 5

In this level the pasword is stored in human readble file inhere dictionary.
to get acces to the pasword we to first cd inhere and then it gives a list of multiple file and to get the pasword we have to 
use the code "file ./"filename"" for each of the file which takes a lot of time but to get the file faster we use the code 
"for i in $(ls); do file ./$i; done" which uses a for loop for the as ls list the file for inhere files and iterates throughout 
the loop  using the code "file ./" for all the list which is stored in i and is given to us as we can see -file007 is ASCCI text 
which has the passord inside we can then directly code "cat ./-file007" which gives us password.

## level 5->6

in this level the password is hdden inhere file with 3 properties.
first we must cd inhere and we can use a code"ls -aRl" which stands for all recursive list for inhere file but we get to many long file 
and to get into 1 file at a time is very time consuming so we use a code "find . -readable -size 1033c -not -executable" and this code 
searches throught the files which is human readable and has sie 1033c where c is bytes and is not executable and we get the file and have to
just use the "cat "filename".

## level 6 -> 7

in this level the pasword is somewhere in the server which has 3 properties.
to get inside the server we can use the code "find /" which means it gets us into the server or root user and the full code is 
"file / "file properties"" which gives us files which have permission denied but we see that there is a file which doesnt get 
permission denied and to get this file we use code "find / -user bandit7 -group bandit6 -size 33c 2>/dev/null" where the null will 
store all the permission denied file and we can get the file which has password and we can just use "cat "file name"" to get the password.

## level 7 -> 8

in this level the pasword is in the file data.txt next to the word millionth.
to get the password we use the code ls to give the list of file and we get file data.txt and if we use the code "cat data.txt" we can
see that it gives us many list of file and we cannot locate millionth to get millionth we use the code "cat data.txt | grep "millionth"" 
as this code cat will give output of data.txt and the tool grep is a tool in linux which helps us search the word we are looking which is 
"millionth " and hecne we get the password.

## level 8 -> 9

in this level the pasword is in file called data.txt which has 10001 lines of pasword which can be found using code "wc -l data.txt" and 
the pasword is unquie where it is no repeated .
to find the password we have to use the code "cat data.txt |sort |uniq -c " which gives us the sorted pasword all unquie differntly and the code 
c is crown where it shows us how much number of times it repeated but we get again to many lines of password which is repeated 10 times and we
 get to see 1 password which is repeated once so to get that password which is not repeated can be found using code
  "cat data.txt |sort |uniq -c |grep -v 10" where the tool grep is used for finding a particular word but -v stands for not so grap -v 10 means
  not to give 10 repeated password so hence we get the password.

## level 9 -> 10

in this level the pasword is hidden in file data.txt where it is in one of few human readable strings with starting word with 
several equal to sign "=====" .
to find the pasword we can use ls where we get data.txt and the wc -l data.txt will give us 67 data.txt and to get few human readle
strings we use the code "strings data.txt" where strings means human readable to show output of data.txt but we get many lines so to find 
the password we use the code "strings data.txt | grep =" which will fetch us the line which has equal to sign"=" because of grep tool 
and from there we can see that the line which starts with several equal to sign "====" is the pasword.

## level 10 -> 11

in this level the pasword is in data.txt where it encoded in 64 encoded data.
Base64 encoding is a method used to encode binary data into ASCII characters. It's commonly used in various applications and protocols, such 
as email attachments, storing complex data in XML, and transmitting data over the Internet, among others. The term "64" in Base64 refers to the 
number of characters in its alphabet, which includes uppercase and lowercase letters, digits, and two additional symbols.
to get the password we use the code "cat data.txt" to get outpyut in 64 enocoded data  we have to decode the 64 encoding data by using the code 
"cat data.txt | base64 -d" which decodes the 64 encoding data base64 -d is a linux installed language which decodes and gives us the password.

## level 11 -> 12

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 
positions.
to get the passsword we can use "cat data.txt" which gives us the passord which is in all lowercase (a-z) and uppercase (A-Z) letters have
 been rotated by 13 and to unroatate it 13 times we can go to rot13 website where it will unrotate all the words 13 times and give us the 
the password.

## level 12 -> 13

The journey from Bandit Level 12 to Level 13 was a fascinating exploration into the intricacies of data compression and encoding, underscoring the 
importance of proficiency in command-line tools for data manipulation and analysis within Unix-based systems.

Beginning with the discovery of the data.txt file, which initially appeared as binary gibberish, the process unfolded into a series of iterative 
decoding and decompression tasks. Leveraging commands like xxd, file, and various compression utilities such as gzip and bzip2, each layer of the 
data was meticulously peeled away, revealing deeper insights into its structure and contents.

This exercise underscored the significance of persistence and adaptability in problem-solving within the realm of cybersecurity. The need to navigate
 through multiple layers of data compression and encoding mirrored real-world scenarios where adversaries might employ similar tactics to obfuscate sensitive information.

Moreover, the experience reinforced the value of a methodical approach to problem-solving, emphasizing the importance of thorough analysis and experimentation 
to uncover hidden insights effectively. Each step of the process required careful consideration and experimentation with different commands and techniques, highlighting the
 dynamic nature of cybersecurity challenges.

 ## level 13 -> 14

in this level i have to login as user bandit and to login as bandit user14 i have to use the localhost hostname which is
"ssh bandit14@localhost -p 2220 -i sshkey.private" which makes me login as user as i am using ssh key to login to localhost 
with pasword -p 2220 and giving my identity as sshkey.private so that i can enter as user.
after getting login as user the password is easy to find as the code is already given in instruction with code 
"cat /etc/bandit_pass/bandit14 " which gives us the password.

## level 14-> 15

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.
we can get the pasword by using a code "nc" called versatile networking tool that reads and writes data across network 
connections and the command "nc localhost 30000"  used to establish a network connection to a server running on the local 
machine (localhost) via the specified port number and then we are meant to enter the password for the level 14 and we get 
the password for the next level.

## level 15 ->16

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost 
using SSL encryption.
so to get the password for next level we hace to be be on the same server with the client with the same server
using the code "pass=jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt;openssl s_client -connect localhost:30001" which makes us on the same 
server with client and we have to enter the previuos level password and will be granted with the next level password.

## level 16 -> 17

the password for the next level is stored in a file named sshkey.private on the localhost.
we have to use nmap of localhost in the instruction to find the server and then use nmap to find the server version to find the 2 server.
Connect to the Bandit server using SSH..
Transfer the contents of sshkey.private to your local machine.
Extract the private key from sshkey.private.
Use the private key to SSH into the Bandit server as the next level user.

## level 17 -> 18

there is two passwords  and he password for the next level is in passwords.new and is the only line that has been changed between passwords.old 
and passwords.new.
to get the password we use a code "diff passwords.old passwords.new" where the function diff tells us the differnce betweeen password.old and password.new 
and tells which is added and changed line so we are shown which is added and changed and hene we get thr passowrd.

## level 18 -> 19

in this level the password is in readme file but we unable to login in level 18 .
to get the password we can use the code which we login in the level "shpass -p$(cat 18) ssh bandit18@bandit.labs.overthewire.org -p 2220"  and add ls on the last
word like "shpass -p$(cat 18) ssh bandit18@bandit.labs.overthewire.org -p 2220 ls" to give the list of the level which gives us the file 
readme and to open the file without entering the level i can use the code like same "shpass -p$(cat 18) ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme" 
where the cat code will give me the output password.

## level 19 ->20

After logging into bandit19�s profile, I ran "ls" and I saw the binary file named "bandit20-do". The hint stated that I needed to execute the file, so I did with the
 "./bandit20-do" command. The output said "Run a command as another user. Example: ./bandit20-do id". I then ran "./bandit20-do id" and I was able to see bandit20�s id 
 information. The script seem to do what it said "run a command as another user". Since the password for bandit20 is in the "/etc/bandit_pass/" I decided to run
  "./bandit20-do cat /etc/bandit_pass/bandit20" since only bandit20 is able to read the file. The result was that I was able to see the next password.