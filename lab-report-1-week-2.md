# Lab Report 1 - Week 2 
## How to utilize course-specific account on ieng6
## Yonghyeon Choi PID:A17010613

**Part1 : Installing VScode**
- First of all, go to [Visual Studio Code Website](https://code.visualstudio.com/). Follow all the steps.
- Install the VScode in your Mac, Windows, or Linux. 
- Image below will be a window that you will see if you have installed the program properly on your device. 

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/59759c8eae231ffcfda73fd2e6f6397e25b40b01/Lab1%20-%201.png)

**Part2 : Remotely Connecting**
- Collaborating with others when working on a same project can be done easily by setting your device capable to connect to a remote computer. 
- We are going to connect to remote computer by using our CSE15L course-specific accounts. 
- First, go to [UCSD ETS](https://sdacs.ucsd.edu/~icc/index.php), where you can find your course account.
- Type in your name and PID, and change your password. Now, you know your own course-specific account and password to log in.
- Open a new terminal in VScode, and type in "ssh (your account)". 
- It will tell you that the authenticity of host can't be established and ask you if you still want to connect. Type in "yes".
- It will ask you to type in your password. It is normal that what you type in doesn't show up on your screen. 
- If you have successfully logged in to a remote computer, you will see a screen like below.

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/14855a1b5bedbfab25ef17ee0d6103fbb4b04bad/Lab1%20-%202.png)

**Part3 : Trying Some Commands**
- Now you have logged into the remote computer.
- Here are some commands that you can try. 
- cd ~ 
- cd (cd command changes the current directoy into other system)
- ls -lat 
- ls -a (ls command lists all the the files in the current directory) 
- exit (this command lets you log out)
- Image below is what you will likely see if you try some of these commands. 

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/14855a1b5bedbfab25ef17ee0d6103fbb4b04bad/Lab1%20-%203.png)

**Part4 : Moving Files with scp**
- Moving various files bewteen local and remote computers is a critical benefit that working remotely has.
- Command called "scp" lets you do this. Create a random java file on your local computer and run it using "javac" and "java" commands. 
- Now type in "scp (file name) (your account address)". Then, type in your password. 
- Log in to your account, then use command "ls" to check that the file you created on your local computer has been copied into the remote computer.
- You can run that program on the remote computer now. It means anyone on the server can run the program.
- Image below shows the demonstration.

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/14855a1b5bedbfab25ef17ee0d6103fbb4b04bad/Lab1%20-%204.png)

**Part5 : Setting an SSH Key**
- It takes time for you to type in your password everytime you log in the remote computer.
- To make this progress more convenient, you can use "ssh" keys. 
- A program called "ssh-keygen" creates a public key and private key. Private key is copied on the client and public key is copied on the server. 
- It lets you to log in to the remote computer without typing in your password everytime. 
- It means that you can use commands like ssh and scp without entering your password also.
- Image below shows how to set it up.

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/14855a1b5bedbfab25ef17ee0d6103fbb4b04bad/Lab1%20-%205.png)

**Part6 : Optimizing Remote Running**
- There are lots of ways to optimize remote running.
- For example, using command in quotes at the end of ssh command to immediately run it on the server.
- Upside arrow brings the previous command line you typed in. 
- Semicolons let you run multiple commands in one command line. Image below is a demonstration. 

![Image](https://github.com/choi8616/cse15l-lab-reports/blob/14855a1b5bedbfab25ef17ee0d6103fbb4b04bad/Lab1%20-%206.png)
