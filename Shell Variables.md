# Shell Variables
## Printing Variables
used the command `echo $FLAG` to print the flag.
## Setting Variables
used the command `PWN=COLLEGE` to assign the value college to pwn variable and obtained the flag. 
## Multi-word Variables
used the command `PWN="COLLEGE YEAH"` to assign the value college to pwn variable and obtained the flag.
## Exporting Variables
First, we assign the value of the variable PWN to COLLEGE and the value of the variable COLLEGE to PWN. Next, we export the variable PWN to the shell using the command `export PWN`. Finally, we open a shell and execute the command `/challenge/run` to obtain the flag.

Flag: pwn.college{ITidK1ADV7Ps9lUALfXPjHfL9d7.dJjN1QDL2kzM2czW}
## Printing Exported Variables
Used the `env` command to print every exported variable in the shell

Flag: pwn.college{8ahAvdN0nyTO-yVSU6V5YKsnHxg.dhTN1QDL2kzM2czW}
## Sorting Command Output
We assign the variable PWN with the output of the command /challenge/run using the following syntax: `PWN=$(/challenge/run)`

To read the contents of the variable, we use the command: `echo $PWN`

Flag: pwn.college{4enOiTjZQ-b6Zd2uFh4-jwwgCCP.dVzN0UDL2kzM2czW}
## Reading Input
We can use the command `read -p "input:" PWN` to prompt for input and enter `COLLEGE` when prompted. This will provide us with the flag.

Flag: pwn.college{ARwi-4k232WaEgUzUetkbnK6lzf.dhzN1QDL2kzM2czW}
## Reading Files


Flag: pwn.college{MT10OZxfwo8k3PoFO2P6uUF2P3g.dBjM4QDL2kzM2czW}
