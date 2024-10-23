# Processes and Jobs
## Listing Processes
To obtain the flag, we first list the currently running processes using the `ps -ef` command to identify the renamed version of `/challenge/run`. This will reveal the new file name, such as `/challenge/17758-run-23919`.

Flag: pwn.college{Undt422KTY-c1OkcpjgX1k7DXmE.dhzM4QDL2kzM2czW}
## Killing Processes
To obtain the flag, we need to locate the `dont_run` process as instructed. First, we run the `ps -ef` command to list all processes. Among them, we identify the process labeled `sleep` with a PID of 74. We then terminate this process using the command `kill 74`. After that, we can execute `/challenge/run` to retrieve the flag.

Flag: pwn.college{wc_dVIzPJ1N1CdFQNBh9Sfn2QiP.dJDN4QDL2kzM2czW}
## Interrupting Processes
To get the flag, execute the command `/challenge/run` to start the process, then press `Ctrl + C` to interrupt it. This will display the flag.

Flag: pwn.college{M0zcDLq821VyKeOXSvbWQzBY8h7.dNDN4QDL2kzM2czW}
## Suspending Processes
To get the flag, execute the command `/challenge/run` to start the process, then press `Ctrl + Z` to suspend it. This will display the flag.

Flag: pwn.college{sJmnYu9ewuA4fpMdy0RzTkEIwgl.dVDN4QDL2kzM2czW}
## Resuming Processes
To obtain the flag, start the process by running the command `/challenge/run`, then suspend it by pressing `Ctrl + Z`. After that, resume the process with the `fg` command to reveal the flag.

Flag: pwn.college{A5gDPBJ2N5k5Hjg997Zzil-jCjT.dZDN4QDL2kzM2czW}
## Backgrounding Processes
To acquire the flag, begin by running the process `/challenge/run`. Press `Ctrl + Z` to suspend it, then use the `bg` command to resume it in the background. After that, start another instance of `/challenge/run` to obtain the flag.

Flag: pwn.college{oH-la19GFn82gwuxCAbpB7gXvRN.ddDN4QDL2kzM2czW}
## Forgrounding Processes
To obtain the flag, first start the `/challenge/run` process by running the command. Then, suspend the process with `Ctrl + Z`. Resume it in the background using the `bg` command, and finally bring it back to the foreground with the `fg` command to reveal the flag.

Flag: pwn.college{Qmpi9S5k7bsbyXt8wIz43XqwGXF.dhDN4QDL2kzM2czW}
## Starting Backgrounding Processes


Flag: pwn.college{0ZCZmwNTZ-uwPRIuSTlgRAuBEz9.dlDN4QDL2kzM2czW}
## Process Exit Codes
To obtain the flag, start by running `/challenge/get-code`, which will terminate without executing. Next, check the exit code by using the `echo $?` command. Use this exit code as the argument for `/challenge/submit-code`. Finally, execute `/challenge/submit-code 160` to retrieve the flag.

Flag: pwn.college{Iy3VWs9slYd-QcmoWdAjDBdln80.dljN4UDL2kzM2czW}
