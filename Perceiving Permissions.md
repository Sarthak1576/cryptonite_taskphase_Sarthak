# Perceiving Permissions
## Changing File Ownership
To change the user of the flag file located in the root directory, first navigate to the root directory using `cd`. Then, run `ls -l` to view the file details, where you'll see that both the user and group of the flag are set to root. Use the command `chown hacker flag` to change the file's user to hacker. Finally, run `cat flag` to reveal the flag.

Flag: pwn.college{EGl7IVJNeqyk_GhnaUqq514Ujtq.dFTM2QDL2kzM2czW}
## Groups and Files
The flag is located in the root directory. First, navigate to the root directory using `cd`, then run `chgrp hacker flag` to change the file's group from root to hacker. After this, using the `cat` command will display the flag.

Flag: pwn.college{s1_Uv5uRuDOj7H2RschpmfGzw3S.dFzNyUDL2kzM2czW}
