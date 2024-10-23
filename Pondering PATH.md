# Pondering PATH
## The PATH Variable
In this challenge, we clear the `PATH` variable, then execute the `/challenge/run` command. By emptying the `PATH`, the run program is unable to locate the `rm` command, allowing us to keep the flag.

Flag: pwn.college{wKN6rIRzF_RNFiRbBRd1M-gKGLS.dZzNwUDL2kzM2czW}
## Setting PATH
Set the `PATH` variable to the `/challenge/more_commands` directory by running `PATH=/challenge/more_commands`. Then, execute the `/challenge/run` command to successfully run the `win` command.

Flag: pwn.college{MPz1Z4l97tVe_V8q0Irup1S-6xc.dVzNyUDL2kzM2czW}
## Adding Commands
Created a win script that uses `/bin/cat /flag`, make it executable, and place it in your current directory. Then, update the PATH variable to include this directory with `PATH=$(pwd):$PATH` and run `/challenge/run`.

Flag: pwn.college{knO3g7ZCnUZoCEV2eZTzdSmO8Cj.dZzNyUDL2kzM2czW}
## Hijacking Commands
Created `rm` script that uses the command `cat /flag`, make it executable. Then, update the PATH variable to include this directory with `PATH=/home/hacker:$PATH` and run `/challenge/run`.

FLag: pwn.college{A4c4inyDtREsfiYVBPvMDmg5TXv.ddzNyUDL2kzM2czW}
