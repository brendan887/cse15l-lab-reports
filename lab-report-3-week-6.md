# Lab Report 3

## 1. Streamlining `ssh` Configuration
To streamline the remote access process even further, a config can be used.

![Image](screenshots/lab3-1.png)
This config file was created by using `cd ~/.ssh` and `nano config` in Terminal (Mac).

![Image](screenshots/lab3-2.png)
*This shows the creation of `config` and logging into my account using the alias `ieng6`.*

Commands such as `scp` can also be simplified by using the alias.

![Image](screenshots/lab3-3.png)
*`bug1.png` was successfully copied to the server by using the alias.*


## 2. Setting Up Github Access from `ieng6`
To commit and push changes to a Github repository on an remote account, an `ssh` key must be generated.

Public Key on Github:
![Image](screenshots/lab3-4.png)

Public and Private Keys in `ieng6` Account:
![Image](screenshots/lab3-5.png)




## 3. Copy whole directories with `scp -r`

