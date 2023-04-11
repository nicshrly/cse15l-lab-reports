# **Lab Report 1**
## Installing VScode
Follow this link [https://code.visualstudio.com/download](https://code.visualstudio.com/download) then click download for your respective OS and complete the steps for installation.
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20161413.png)


Then, open the VScode application. If your screen looks like the image below, you have completed the installation of VScode.
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20161913.png)


## Remotely Connecting
First, reset the password to your CSE15L Account by following these steps:
1. click this link: [https://sdacs.ucsd.edu](https://sdacs.ucsd.edu/~icc/index.php)
2. enter your username (the same as in your ucsd email) and PID where it says account lookup
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20164019.png)


3. select your cs15l account
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20182259.png)


4. click the link that says "Global Password Change Tool"
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20182522.png)


5. click the link that says "Proceed to the Password Change Tool"
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20182742.png)


6. enter your unique CSE15l account username and follow the steps to reset your password
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20182940.png) 


Once you reset your password, remotely connect by following these steps:
1. if you use windows, download git by going to this link [https://gitforwindows.org](https://gitforwindows.org/), select download, and complete the steps for installation
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20185256.png)


2. open VScode and open a new terminal
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20185717.png)


3. Open the command palette using Ctrl + Shift + P and type and select "Select Default Profile"
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20185917.png)


4. select GitBash
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20190140.png)


5. click on the + icon in the terminal window and the new terminal should be a Git Bash terminal
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20190223.png)

6. in your terminal, enter '$ ssh cs15lsp23zz@ieng6.ucsd.edu' with 'zz' being replaced by the two letters in your course account (you don't type the '$')

7. enter 'yes' if you get the message
'The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established. RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?'


8. when prompted with 'Password:', type in the password you set for your account earlier (nothing will show up as you type in the password, it is not a mistake)


10. if oyu have loghed in successfully, your terminal output should look like this:
![Image](https://github.com/nicshrly/cse15l-lab-reports/blob/main/Screenshot%202023-04-10%20192841.png)

## Using Commands
