# Digesting Documentation
## Learning from documentation
We us the command `/challenge/challenge --giveflag` to get the flag

Flag: pwn.college{IPRFG5cw8Yv0VdILrj0jMIQFbr7.dRjM5QDL2kzM2czW}
## Learning complex usage
changed directory `cd /` and as mentioned in the description, we can use the command  `/challenge/challenge --printfile /flag`, which will display the flag in the terminal.

Flag: pwn.college{UlNp-P6JozWLLGmxwYW_Ty__A1G.dVjM5QDL2kzM2czW}
## Reading manuals
Read the manual with `man challenge` and running the command `/challenge/challenge --gvpctm 064` gave the flag 

Flag: pwn.college{0QgA6LvpJctmy45IIYtPGvKjmHX.dRTM4QDL2kzM2czW}
## Searching Manuals
Read the manual with `man challenge` and used `/ flag` to search and fing the argument to be `--tr`

Flag: pwn.college{ghwaD-QJXOCNbWXg52rE50ayaYN.dVTM4QDL2kzM2czW}
## Searching for manuals
Running the `man man` command, as instructed, opens the manual page for the `man` command. Scrolling down reveals a section called FINDING MANUAL PAGES, where you'll find the `--wildcard` option. This option allows you to search for a specific string across other manual pages.

Used `man --wildcard flag` and then `/challenge/challenge --slkunx 824` to obtain the flag.

Flag: pwn.college{QVG8B-s2HF4lkunxfDve-Tq0KH8.dZTM4QDL2kzM2czW}
## Helpful Programs
used `/challenge/challenge --help` that gave hints in where the flag is. 

The `-g` argument accepts a value and, if it matches the secret value, it prints the flag. Additionally, the `-p` argument displays the secret value.

After the secret value is found by using the `/challenge/challenge -p`, the secret value being 599, used the command `/challenge/challenge -g 599` and got the flag.

Flag: pwn.college{QVnic5hbaObs9UNWpzjfYffuF9D.ddjM4QDL2kzM2czW}
## Help for Bulitins
Used the command help challenge to get information

Given the value for secret is UkbUYiL5 so, used challenge --secret UkbUYiL5 to get the flag.

Flag: pwn.college{UkbUYiL58oizNmtMRzv4JshkuVx.dRTM5QDL2kzM2czW}
