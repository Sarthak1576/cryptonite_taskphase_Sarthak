# Perceiving Permissions
## Changing File Ownership
To change the user of the flag file located in the root directory, first navigate to the root directory using `cd`. Then, run `ls -l` to view the file details, where you'll see that both the user and group of the flag are set to root. Use the command `chown hacker flag` to change the file's user to hacker. Finally, run `cat flag` to reveal the flag.

Flag: pwn.college{EGl7IVJNeqyk_GhnaUqq514Ujtq.dFTM2QDL2kzM2czW}
## Groups and Files
The flag is located in the root directory. First, navigate to the root directory using `cd`, then run `chgrp hacker flag` to change the file's group from root to hacker. After this, using the `cat` command will display the flag.

Flag: pwn.college{s1_Uv5uRuDOj7H2RschpmfGzw3S.dFzNyUDL2kzM2czW}
## Fun with Group Names
In the question, it's mentioned that the group for the user hacker has been changed to a random name. You can find the new group by running the `id` command while in the home directory. After identifying the new group, use the `chgrp` command with the updated group name to gain access to the flag file. Finally, you can use `cat` to reveal the flag.

Flag: pwn.college{MVz0M0i85KYgaf5nWNUlwboo-Pr.dJzNyUDL2kzM2czW}
## Changing Permissions
used the command `chmod +r /flag` to give read permission on the flag file. Once the file is readable, run `cat /flag` to display the flag.

Flag: pwn.college{UCN4DNTzFcndnVKAosi2CSa5-Lz.dNzNyUDL2kzM2czW}
## Executable Files
Used `chmod +x /challenge/run` to make the program executable. Then, run `/challenge/run` to get the flag.

Flag: pwn.college{g3vdfQnD_N3qGkE_5uf1xT6r1f3.dJTM2QDL2kzM2czW}
## Permission Tweaking Practice
After completing the eight rounds of tweaking permission, we are granted permission to modify the flag file with `chmod`. We can now add read permission to the flag and then use the `cat` command to obtain the flag.

Flag: pwn.college{sifTinNFV3yo3s9enf18rCPsL0g.dBTM2QDL2kzM2czW}
## Permissions Setiing Practice
After completing the eight rounds of setting permission, we are granted permission to modify the flag file with `chmod`. We can now add read permission to the flag and then use the `cat` command to obtain the flag.

Flag: pwn.college{oVdgvDCU5ts9I0-xG-wqYoW4Bfn.dNTM5QDL2kzM2czW}
## The SUID Bit
We set the SUID bit by running the command `chmod u+s /challenge/getroot`. Now, when we execute `/challenge/getroot`, it spawns a shell with root privileges, allowing us to use `cat /flag` to retrieve the flag.

Flag: pwn.college{UoyeitwzxldgP0GfERXz34qxjan.dNTM2QDL2kzM2czW}
