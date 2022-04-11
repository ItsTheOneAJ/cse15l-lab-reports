------
# Starting with VS Code and Remote Sign in: (With Images)
------
## Installing VS Code:
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-04-08%20112204.png)
**Steps:**

1. Go to the [VS Code Website](https://code.visualstudio.com/download)
2. Then click install for either your iOS or windows device. 
3. Set up the installation and open the application once available. 


## Remotely Connecting: 
![image](https://github.com/ItsTheOneAJ/jk/blob/main/Screenshot%202022-04-10%20234847.png)
**Steps:**
1. Find your CS 15L account name
2. Enter ssh, and then account name + **@ieng6.ucsd.edu**
3. When prompted for password, enter your new password. 


## Trying Some Commands: 
![image](https://github.com/ItsTheOneAJ/cse15l-lab-reports/blob/main/Screenshot%202022-04-08%20114447.png)
**Steps:**
1. Enter cd ~, ls -lat, cd and other commands
2. See what other things you can do with the commands


## Moving Files with `scp`: 
![image](https://github.com/ItsTheOneAJ/jk/blob/main/Screenshot%202022-04-10%20234725.png)
**Steps:**
1. Create a file that is named WhereAmI.java in VS Code, then save it, once you've done that remotely connect to @ieng6.ucsd.edu
2. enter scp WhereAmI.java "(your username)@ieng6.ucsd.edu:~/"
3. Use the ls command to check if the file is in your directory


## Setting an SSH Key: 
![image](https://github.com/ItsTheOneAJ/jk/blob/main/Screenshot%202022-04-10%20234542.png)
**Steps:**
1. Enter ssh-keygen on your computer, Enter file in which to save the key (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
2. Click enter twice while putting nothing into the passpharase prompt
3.If you’re on Windows, enter:  ssh-keygen -t ed25519, now you can enter and leave without entering a passcode




## Optimizing Remote Running: 
![image](https://github.com/ItsTheOneAJ/jk/blob/main/Screenshot%202022-04-10%20232906.png)
**Steps:**
1. Enter scp WhereAmI.java (username)@ieng6.ucsd.edu:~/; ssh (username)@ieng6.ucsd.edu "javac WhereAmI.java; java WhereAmI" 
2.Enjoy the ease!

------
