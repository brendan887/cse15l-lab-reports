# Lab Report 1

## 1. Installing VSCode
* I downloaded VSCode from the [official website](https://code.visualstudio.com/).
* I followed the instructions to install the software onto my laptop.

![Image](screenshots/Part%202.png)
*Opening VSCode after successfully installing.*


## 2. Remotely Connecting
* Since I'm using a Macbook, I did not have to install OpenSSH.
* The first step is to run the following command to connect to the server: `ssh cs15lsp22ath@ieng6.ucsd.edu`
* Then, I entered my password. Note that the password cannot be seen in the terminal as it is hidden by default.
* Since I connected to the server prior to the lab, I did not have to type 'yes' to the connection message.

![Image](screenshots/Part%203.png)
*Screenshot of terminal after completing all the steps above.*


## 3. Trying Some Commands
* For this task, I tested some commands, namely `cd`, `cat`, and `ls`.
* In the screenshot below, I attempted to list the files in another user's directory.

![Image](screenshots/Part%204.png)
*This command resulted in an error.*

* The outcome makes sense, as if access to certain directories could not be restricted by user, then there would potentially be a lot of data breaches and privacy issues.


## 4. Moving Files with `scp`
* I moved `WhereAmI.java` from my own computer to the server using the `scp` command.

![Image](screenshots/Part%205-2.png)

* Following this, I used the `ls` command in the directory on the server to confirm that the file was moved successfully.

![Image](screenshots/Part%205-3.png)
*I also compiled and ran the program to test more commands.*


## 5. Setting an SSH Key
* To avoid having to enter my password everytime I accessed the server, I can use an SSH key.
* The command `ssh-keygen` generates a public and private key.

![Image](screenshots/Part%206-1.png))

* Following this, I had to create an `.ssh` directory on the server and copy the public key into this directory.

![Image](screenshots/Part%206-2.png)

* I then verified that the key enabled me to access the server from my computer without a password.

![Image](screenshots/Part%206-4.png)

* Initially, I was having difficulty to get the key to work properlly. Even after following the above steps, I still had to enter my password. I had to delete some existing keys on my computer in order to solve this problem.

## 6. Optimizing Remote Running
* To increase the efficiency of remote access even further, additional commands can be added after the `ssh` command, as shown in the screenshot below.

![Image](screenshots/Part%207.png)
*By adding `"ls"` at the end, we avoid having to type it in a separate line.*

* It is also possible to run multiple commands at a time by separating them by semicolons.

![Image](screenshots/Part%207-2.png)
*The above command removes `WhereAmI.class`, compiles `WhereAmI.java`, and runs `WhereAmI`.*