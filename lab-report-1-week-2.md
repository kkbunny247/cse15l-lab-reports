## **LAB 1 REPORT**
#### (A16282947)
<br/>

Hello 15L students! The following is a tutorial on how to log into a course-specific account on ieng6. To do so, we will cover these few tasks:

1. Installing Visual Studio Code
2. Remotely connecting to a UCSD server
3. Inputting commands from your client
4. Moving files with "scp"
5. Setting an SSH key
6. Optimizing remote running

<br/>

### **Step 1:**
#### Installing VScode
Download "Visual Studio Code" from this link: https://code.visualstudio.com/. 

Follow the instructions according to the website; this process will differ depending on if you operate on, for example, OSX or Windows.

![image](Screenshot2022-01-13141746.png)

Your setup should look something like this!
<br/>
### **Step 2:**
#### Remotely Connecting
> FOR WINDOWS USERS ONLY:
- Before getting to the UCSD server, we have to install a program called OpenSSH, which allows us to connect remotely.
- Navigate to "Optional Features" in "Settings." Search and install OpenSSH Client and OpenSSH Server. When you are done, proceed with the next steps!

<br/>

Find your account for the CSE 15L class here: https://sdacs.ucsd.edu/~icc/index.php

The course will be under "Additional Accounts." Locate your account. It will be something similar to this, cs15lwi22**zz**@ieng6.ucsd.edu, except the "zz" will be letters specific to your UCSD account.

Next, open a terminal in Visual Studio Code or open a Command Prompt. Input the following command:

`ssh cs15lwi22zz@ieng6.ucsd.edu`

If the message,<br/>
`"The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? ` comes up, type in yes, press enter, and give your password (it will not appear for security reasons)!

If your screen looks like this, you are ready to move on!

![image](Screenshot2022-01-13175112.png)
<br/>
### **Step 3:**
#### Trying Some Commands


<!-- 

Moving Files with scp
Setting an SSH Key
Optimizing Remote Running
-->