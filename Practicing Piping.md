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
## Redirecting Input
We need to redirect the `PWN` file to `/challenge/run`, but first, `PWN` must contain the word "COLLEGE." To do this, we use the command:

`echo COLLEGE > PWN`

After that, we can redirect the `PWN` file as input to `/challenge/run` using the `<` operator.

Flag: pwn.college{AT_FYqdB1ohaZJzTW32YDuVsbT9.dBzN1QDL2kzM2czW}
## Grepping stored Results
We can redirect the output of `/challenge/run` to `/tmp/data.txt` by the command `/challenge/run > /tmp/data.txt`

Then we can use `pwn.college /tmp/data.txt` to grep for the flag.

Flag: pwn.college{0Jp3lIZ21qSqWkAzN-wY4cLvZI5.dhTM4QDL2kzM2czW}
## Grepping live output
We need to search for the flag in the live output of `/challenge/run`. This can be done by using the `|` operator to pipe the output and then using `grep` to filter for the flag in the same command.

`/challenge/run | grep pwn.college`

Flag: pwn.college{8DmEzz7QYvU3Veidugs3cq5QDqY.dlTM4QDL2kzM2czW}
## Grepping errors
The shell has a `>&` operator, which redirects a file descriptor to another file descriptor. This means that we can have a two-step process to grep through errors: first, we redirect standard error to standard output `2>& 1` and then pipe the now-combined stderr and stdout as normal `|`.

Using the command `/challenge/run 2>&1 | grep pwn.college` we get the flag.

Flag: pwn.college{A53KtYNZw_qJTSxff0EwGle7mZT.dVDM5QDL2kzM2czW}
## Duplicating piped data with tee
We need to intercept the `pwn` file to determine the correct arguments to pass to `/challenge/pwn` in order to obtain the flag.

To do this, we use the following command: `/challenge/pwn | tee output.txt | /challenge/college`

This allows us to capture the output in `output.txt`. We can then view the file's contents using `cat`.

Following the instructions in the file leads to the flag:  `/challenge/pwn --secret "I5aFDklv" | /challenge/college`

Flag: pwn.college{I5aFDklvLiSrxY34o-nls9_QMRh.dFjM5QDL2kzM2czW}
## Writing to multiple programs
We use the `tee` command to write the output generated by `/challenge/hack` to both `/challenge/the` and `/challenge/planet` simultaneously with the following command: 

`/challenge/hack | tee >(/challenge/the) >(/challenge/planet)`

Flag: pwn.college{w2HnVEQf23fRRFXJR2Zco1Pbt-Q.dBDO0UDL2kzM2czW}
## Split piping stderr and stdout
The `/challenge/hack` program needs to write its stdout to `/challenge/planet` and its stderr to `/challenge/the`. We can achieve this by redirecting the stdout and stderr using named pipes as follows:

`/challenge/hack > >(/challenge/planet) 2> >(/challenge/the)`

Flag: pwn.college{8t-0vkIXRzE3jmxfZ5kYDhItSue.dFDNwYDL2kzM2czW}

Flag: pwn.college{8t-0vkIXRzE3jmxfZ5kYDhItSue.dFDNwYDL2kzM2czW}
