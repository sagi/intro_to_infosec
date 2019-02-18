# 17/02/2018 - 8th Lecture


## Test #1 - Networking Fundamentals
We've had our first test. You'll your grade next lesson.


## Linux Command Line (bash)

We've learned and used the following commands:

~~~
chmod +x <filename>
chmod <number - e.g. 755>  <filename>
./<executable file>
ls -l
ls -a - list hidden files and directories (start with a ".")
pwd - print working directory
cd - change directory
cd ~ - go to home directory
cd .. - go one directory back
cat <file> - print the file content to stdout
mkdir - make a new directory
touch <filename>  - create a new empty file
rm <filename> - remove a file
mv <f1> <dir / f2> - move f1 to f2 / dir
ln -s <target> <link_name>
whoami - which user is logged in
file <file>  - determine file type
sudo <command> run command from a high privilege context
alias <cmd>="cmd arg1 arg2"
~~~

## DAC - Discretionary Access Control

We've described  Linux's DAC model and played with it.


We also explained MAC (Mandatory Access Control) and described how it hardens
process / file permissions every further.


## Magic Numbers

We've seen that most binary file format starts with their own magic number
which allows operating systems to know the actual type of a file - regardless
of its extension.

We've used the `file` command to check the types of files.

## Pastebin and Sprunge

We've explained the value of services such as Pastebin and Sprunge.

We also tried to add an alias for Sprunge. We'll finish it next lesson :)


## Homework

1. Do HTML Dog's Beginner, Intermediate and Advanced HTML tutorials: [http://www.htmldog.com/guides/html/](http://www.htmldog.com/guides/html/).
You can also do the CSS ones: [http://www.htmldog.com/guides/css/](http://www.htmldog.com/guides/css/).

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. Research and public speaking; find a topic - either a technologoy (e.g. DNS, DHCP)
or a security-related news article and prepare a 2-3 minute talk about it.

5. FOLLOW YOUR FELLOW CLASS MATES: http://bit.ly/2B87gDw with your Twitter, Github and Linkedin.

6. Find relevant job descriptions (e.g. SOC Analyst). Put them in Google Docs.
Highlight the different technologies that are required.

7. Add a new command with `alias`, the command should print your name. Put the alias
in the  ~/.bashrc file and do (in the same terminal) `$ source ~/.bashrc`

8. Work on your CV. In English. Print it for me to review.

9. Find the magic number of three file types, verify it with `hexdump`, then
write them down for next lesson.

10. What does `$ chmod 755` mean? What does `$ chmod 666` mean?


<hr>
Copyright 2019 Sagi Kedmi
