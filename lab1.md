# **Lab Report 1**
## Installing VScode
Follow this link [https://code.visualstudio.com/download](https://code.visualstudio.com/download) then click download for your respective OS and complete the steps for installation.
![Image](Screenshot%202023-04-10%20161413.png)


Then, open the VScode application. If your screen looks like the image below, you have completed the installation of VScode.
![Image](Screenshot%202023-04-10%20161913.png)


## Remotely Connecting
First, reset the password to your CSE15L Account by following these steps:
1. Click this link: [https://sdacs.ucsd.edu](https://sdacs.ucsd.edu/~icc/index.php)
2. Enter your username (the same as in your ucsd email) and PID where it says account lookup
![Image](Screenshot%202023-04-10%20164019.png)


3. Select your cs15l account
![Image](Screenshot%202023-04-10%20182259.png)


4. Click the link that says "Global Password Change Tool"
![Image](Screenshot%202023-04-10%20182522.png)


5. Click the link that says "Proceed to the Password Change Tool"
![Image](Screenshot%202023-04-10%20182742.png)


6. Enter your unique CSE15l account username and follow the steps to reset your password
![Image](Screenshot%202023-04-10%20182940.png) 


Once you reset your password, remotely connect by following these steps:
1. If you use windows, download git by going to this link [https://gitforwindows.org](https://gitforwindows.org/), select download, and complete the steps for installation
![Image](Screenshot%202023-04-10%20185256.png)


2. Open VScode and open a new terminal
![Image](Screenshot%202023-04-10%20185717.png)


3. Open the command palette using Ctrl + Shift + P and type and select "Select Default Profile"
![Image](Screenshot%202023-04-10%20185917.png)


4. Select GitBash
![Image](Screenshot%202023-04-10%20190140.png)


5. Click on the + icon in the terminal window and the new terminal should be a Git Bash terminal
![Image](Screenshot%202023-04-10%20190223.png)

6. In your terminal, enter `$ ssh cs15lsp23zz@ieng6.ucsd.edu` with `zz` being replaced by the two letters in your course account (you don't type the `$`)

7. Enter `yes` if you get the message:
`The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established. RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?`


8. When prompted with `Password:`, type in the password you set for your account earlier (nothing will show up as you type in the password, it is not a mistake)


10. If you have logged in successfully, your terminal output should look like this:
![Image](Screenshot%202023-04-10%20192841.png)

## Using Commands
Next, you should try running some commands on the terminal. Here are some commands you can try and a short description of what they do:
- `pwd`: displays the path to your current working directory

![Image](lr1_p3.png)


- `ls <path>`: displays a list of the files and folders in the given path

![Image](lr1_p3.2.png)


- `cat <path1> <path2>`: displays the contents of one or more files given by the paths

![Image](lr1_p3.3.png)


- `cd <path>`: switches the current working directory to the given path. (nothing will show up when you run this command so to see if it actually worked, you can use the command `pwd` after)

![Image](lr1_p3.5.png)
