# Untangling Users
## Becoming root with su
We execute the `su` command, and when prompted for a password, we enter hack-the-planet. This opens a root shell, allowing us to run the `cat /flag` command to retrieve the flag.

Flag: pwn.college{ghvMF1A-T-aNmqX4XeGEDm3JUkL.dVTN0UDL2kzM2czW}
## Other users with su
Switched to zardus user using `su zardus` and then entered the password, dont-hack-me .Then we obtain the flag by running `/challenge/run`.

Flag: pwn.college{4mSzFDtC4KWmlC5QxbmeL6V85jK.dZTN0UDL2kzM2czW}
## Cracking passwords
Used John the Ripper to crack the password hash `john /challenge/shadow-leak`. Once the password is cracked, use the `su` command to switch to the zardus user and enter the cracked password when prompted. Finally, run the following command to get the flag `/challenge/run`.

Flag: pwn.college{wvddLXr6oZWqKl94Hhx_UbFSN7B.ddTN0UDL2kzM2czW}
