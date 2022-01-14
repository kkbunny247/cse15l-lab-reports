## **Lab 1 Report**
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
<br/>

Download "Visual Studio Code" from this link: https://code.visualstudio.com/. 

Follow the instructions according to the website; this process will differ depending on if you operate on, for example, OSX or Windows.

![image](Screenshot2022-01-13141746.png)

Your setup should look something like this!
<br/>
<br/>
### **Step 2:**
#### Remotely Connecting
<br/>

> FOR WINDOWS USERS ONLY:
- Before getting to the UCSD server, we have to install a program called OpenSSH, which allows us to connect remotely.
- Navigate to "Optional Features" in "Settings." Search and install OpenSSH Client and OpenSSH Server. When you are done, proceed with the next steps!

<br/>

Find your account for the CSE 15L class here: https://sdacs.ucsd.edu/~icc/index.php

Then, in Visual Studio Code, we are going to connect to the remote computer using VSCode’s remote option. For reference, we’re following the steps in “Connect to a remote host” step.

For the first step, open a terminal in VSCode (Ctrl or Command + `, or use the Terminal → New Terminal menu option). Your command will look like this, but with the zz replaced by the letters in your course-specific account.

$ ssh cs15lwi22zz@ieng6.ucsd.edu
(That’s one, five, l (not one); the one and l look very close in some fonts.)

Since this is likely the first time you’ve connected to this server, you will probably get a message like this:

⤇ ssh cs15lwi22zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
I (Joe) always say yes to these messages when I’m connecting to a new server for the first time; it’s expected to get this message in that case. If you get this message when you’re connecting to a server you connect to often, it could mean someone is trying to listen in on or control the connection. This answer is a decent description of what’s going on: Ben Voigt’s answer

So type yes and press enter, then give your password; the whole interaction should look something like this once you give your password and are logged in:

⤇ ssh cs15lwi22zz@ieng6.ucsd.edu
The authenticity of host 'ieng6-202.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
Password: 
Last login: Sun Jan  2 14:03:05 2022 from 107-217-10-235.lightspeed.sndgca.sbcglobal.net
quota: No filesystem specified.
Hello cs15lwi22zz, you are currently logged into ieng6-203.ucsd.edu

You are using 0% CPU on this system

Cluster Status 
Hostname     Time    #Users  Load  Averages  
ieng6-201   23:25:01   0  0.08,  0.17,  0.11
ieng6-202   23:25:01   1  0.09,  0.15,  0.11
ieng6-203   23:25:01   1  0.08,  0.15,  0.11

Sun Jan 02, 2022 11:28pm - Prepping cs15lwi22
Now your terminal is connected to a computer in the CSE basement, and any commands you run will run on that computer! We call your computer the client and the computer in the basement the server based on how you are connected.

If, in this process, you run into errors and can’t figure out how to proceed, ask! When you ask, take a screenshot of your problem and add it to your group’s running notes document, then describe what the fix was. If you don’t know how to take a screenshot, ask!

Remember – it is rare for a tutorial to work perfectly. We often have to stop, think, guess, Google search, ask someone, etc. in order to get things to work the way the tutorial says. I look up the right way to describe the (yes/no) answer on first login all the time, for example. So you are helping your group learn about potential issues when you do this, and that’s a major learning outcome of the course! If you see someone else have an issue that you didn’t, ask why, and what might be different about what you did, or how your environment is set up. You will learn by reflecting on this.

Write down in notes When you’re done, discuss what you saw upon login. Take a screenshot or copy/paste the output. Did you all see the same thing? What might the differences mean? Note the results of your discussion in the notes document.


<!-- 



Trying Some Commands
Moving Files with scp
Setting an SSH Key
Optimizing Remote Running
-->