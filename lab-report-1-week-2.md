# Lab Report 1 - Week 2 
## How to utilize course-specific account on ieng6
## Yonghyeon Choi PID:A17010613

**Part1 : Installing VScode**
- First of all, go to [Visual Studio Code Website](https://code.visualstudio.com/). Follow all the steps.
- Install the VScode in your Mac, Windows, or Linux. 
- Image below will be a window that you will see if you have installed the program properly on your device. 

![Image](Lab1 - 1.png)

**Part2 : Remotely Connecting**
- Collaborating with others when working on a same project can be done easily by setting your device capable to connect to a remote computer. 
- We are going to connect to remote computer by using our CSE15L course-specific accounts. 
- First, go to [UCSD ETS](https://sdacs.ucsd.edu/~icc/index.php), where you can find your course account.
- Type in your name and PID, and change your password. Now, you know your own course-specific account and password to log in.
- Open a new terminal in VScode, and type in `ssh (your account)`. 
- It will say `the authenticity of host can't be established` and ask you if you still want to connect. Type in `yes`.
- It will ask you to type in your password. It is normal that what you type in doesn't show up on your screen. 
- If you have successfully logged in to a remote computer, you will see a screen like below.

![Image](Lab1 - 2.png)

**Part3 : Trying Some Commands**
- Now you have logged into the remote computer.
- Here are some commands that you can try. 
- `cd ~` 
- `cd` (cd command changes the current directoy into other system)
- `ls -lat` 
- `ls -a` (ls command lists all the the files in the current directory) 
- `exit` (this command lets you log out)
- Image below is what you will likely see if you try some of these commands. 

![Image](Lab1 - 3.png)

**Part4 : Moving Files with scp**
- Moving various files bewteen local and remote computers is a critical benefit that working remotely has.
- Command called `scp` lets you do this. Create a random file on your local computer and run it using `javac` and `java` commands. 
- Now type in `scp (file name) (your account address)`. Then, type in your password. 
- Log in to your account, then use command `ls` to check that the file you created on your local computer has been copied into the remote computer.
- You can run that program on the remote computer now. It means anyone on the server can run the program.
- Image below shows the demonstration.

![Image](Lab1 - 4.png)

**Part5 : Setting an SSH Key**
- It takes time for you to type in your password everytime you log in the remote computer.
- To make this progress more convenient, you can use `ssh` keys. 
- A program called `ssh-keygen` creates a *public key* and *private key*. Private key is copied on the client and public key is copied on the server. 
- It lets you to log in to the remote computer without typing in your password everytime. 
- It means that you can use commands like `ssh` and `scp` without entering your password also.
- Image below shows how to set it up.

![Image](Lab1 - 5.png)

**Part6 : Optimizing Remote Running**
- There are lots of ways to optimize remote running.
- For example, using command in quotes at the end of `ssh` command lets you immediately run it on the server.
- *Upside arrow* brings the previous command line you typed in. 
- *Semicolons* let you run multiple commands in a single command line. Image below is a demonstration. 

- I went through the process of making a change in `WhereAmI.java`, moving file over `ssh` with `scp`, logging in with `ssh`, checking with `javac` and `java` commands, and finally exiting with `exit` command without any optimization. *121* keystrokes were involved during this process. 
- Then, I went through the same process utilizing the up-arrow key. *17* keystrokes were involved this time. I tried using command in quotes at the end of `ssh` or semicolons, but using only up-arrow key was most efficient in decreasing the number of keystrokes.

![Image](Lab1 - 6.png)
