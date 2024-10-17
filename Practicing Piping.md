# Practicing Piping
## Redirecting Output
Used input redirection to write the word PWN to the filename COLLEGE with the command `echo PWN > COLLEGE` and got the flag.

Flag: pwn.college{kOI1A4lwrYyOZgbLnQR97bugPrO.dRjN1QDL2kzM2czW}
## Redirecting more Output
Executing the command `/challenge/run > myflag` replaces the contents of the myflag file with the output of `/challenge/run`. 

After that, using the `cat` command on the `myflag` file will display the flag.

Flag:pwn.college{ka1RAdU6LY_LmSXTIMSNYtUkJlk.dVjN1QDL2kzM2czW}
## Appending Output
Executing the command `/challenge/run >> /home/hacker/the-flag` appends the first half of the flag directly to the file, followed by appending the second half through the stdout.

After that, using the `cat` command on the `/home/hacker/the-flag` file will display the flag.

Flag: pwn.college{UY-nEc_KBBGGDTwodxwB5rEOIuM.ddDM5QDL2kzM2czW}
## Redirecting Output
We run the command `/challenge/run` with `1> myflag` to direct the stdout output to the `myflag` file, and `2> instructions` to send output to the instructions file. Afterward, using the `cat` command on `myflag` will display the flag.

Flag: pwn.college{ka1RAdU6LY_LmSXTIMSNYtUkJlk.dVjN1QDL2kzM2czW}
