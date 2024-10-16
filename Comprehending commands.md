# Comprehending Commands
## cat, not the pet, but the command 
Used `ls` command to check what files are present, and used the `cat` command to read the file flag to obtain the flag

Flag: pwn.college{UgrlVwota0KqYaa7Tov9kZLHLB0.dFzN1QDL2kzM2czW}
## catting absolute paths
Used `cat /flag` command to obtain the flag

Flag: pwn.college{QTzWZfwDXPhmoIKbHLnlZZjK41a.dlTM5QDL2kzM2czW}
## more catting practice
Used `cd flag` command to obtain the path to the flag. After obtaining the path `/lib/x86_64-linux-gnu/avahi/flag` used the `cat` command to read and obtain the flag

Flag:pwn.college{E1oswrC-G3DvlhfbbWdxY0d-uW6.dBjM5QDL2kzM2czW}
## grepping for a needle in a haystack
Used `grep pwn.college /challenge/data.txt` command to obtain the flag in the file with thousand lines.\ and specified pwn.college in the command for the flag. 

Flag: pwn.college{wRA6n1Kp5MJir1L-22MT7jkxQPy.ddTM4QDL2kzM2czW}
## listing files
Used `cd /challenge` command then `ls` to see where the flag is, and then used `/challenge/22060-renamed-run-32203` to obtain the flag

Flag: pwn.college{MAxgRcw6uvqgwrRzdMBRMApcbV9.dhjM4QDL2kzM2czW}
## touching files
Created two files /tmp/pwn and /tmp/challenge using the `touch` command and then the `/challenge/run` command to obtain flag.

Flag:pwn.college{EwGPZmtcMrAAWK1ijEbUwscLnco.dBzM4QDL2kzM2czW}
## removing files
Removed the file delete_me with the `rm` command and used `/challenge/check` to obtain flag

Flag: pwn.college{AUx6xMVC6j5cvqQuOdeXyPH_M2t.dZTOwUDL2kzM2czW}
## hidden files
Changed the directory by using `cd /` then used `ls -a` command to find the hidden files. After that used the `cat` command to read the file and get the flag.

Flag: pwn.college{o5mwkc0bpyzPPvFHir3njYGQ2ZM.dBTN4QDL2kzM2czW}
## An epic filesystem quest
Using the commands learnt such as `ls`, `ls -a` and `cat` and getting multiple clues finally got the flag.

Flag: pwn.college{URwc0GYoMUrOZY1nIIYWWbgqdY-.dljM4QDL2kzM2czW}
## making directories
created directories using `mkdir` and created a file using `touch` then used `/challenge/run` to get flag.

Flag: pwn.college{QvTYl7RXY3xtKgUqmZQF4NEhBTY.dFzM4QDL2kzM2czW}
## finding files
used command `find / -name flag -type f` and obtained the path and read it with `cat`.

Flag: pwn.college{0xhC84g0VcPvYAH6qhF30452zdl.dJzM4QDL2kzM2czW}
## linking files
In this challenge, we need to create a symbolic link between the `/flag` file, which contains the flag, and the `/not-the-flag` file, which is executed by the given command. By using `ln -s` to create the symbolic link and then running the provided command, we can retrieve the flag.

Flag: pwn.college{IrIXnfnO_k6gxpeb04HBhIcxfHu.dlTM1UDL2kzM2czW}
