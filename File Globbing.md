# File Globbing
## Matching with *
Given we can use only four characters. Thus we use globbing and use the command `cd ch*` to enter in the challenge directory.

Ran `/challenge/run` to obtain the flag.

Flag: pwn.college{MpxzM90fiw2xCJTinaBqYZ5uc9E.dFjM4QDL2kzM2czW}
## Matching with ?
Considering the constraints, we need to navigate to the challenge directory by using `?` in place of the letters c and l.

Used `?` in the command `cd /?ha??enge` and then the `/challenge/run` command.

Flag: pwn.college{wGEtJZH56blzlSPQYpF9BBy_jll.dJjM4QDL2kzM2czW}
## Matching with []
Changed the directory using `cd /challenge/files` and then run the `/challenge/run file_[bash]` accordingly to the given constraints and got the flag.

Flag: pwn.college{IDIert1KCA3wpmb1ROtPvO27lfu.dNjM4QDL2kzM2czW}
## Matching paths with []
Did the same thing as the previous challenge but did it without changing the directory and giving the path `/challenge/run /challenge/files/file_[bash]`

Flag: pwn.college{IwqGkAtnCHErt3KXmRFnVXvtXV0.dRjM4QDL2kzM2czW}
## Mixing Globs
Changed the directory using `cd /challenge/files` and then run ls to check the files and used `/challenge/run [cep]*` to get the flag.

Flag: pwn.college{kwBcKsMrYFVzoS1KO0BFsKTrLbn.dVjM4QDL2kzM2czW}
## Exclusionary globbing
Changed the directory using `cd /challenge/files` and then run the `/challenge/run [pwn]*` accordingly to the given constraints and got the flag.

Flag: pwn.college{8pkJ8pANqb9XxvefKWjiS8nXodo.dZjM4QDL2kzM2czW}
