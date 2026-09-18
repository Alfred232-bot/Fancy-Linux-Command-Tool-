# Fancy-Linux-Command-Tool-

Section 1 - Command Description

What My Tool Does
My tool is a simple "fancy" Linux command that combines two common Linux commands into one tool.
The tool combines grep and head. It searches a text file for a specific word or pattern and then displays only the first few matching lines.
This makes it easier to quickly find information in a large text file without having to run multiple commands separately.

Commands Combined
The two Linux commands used are:
• grep — searches for a specific word or pattern in a file.
• head — displays the first lines of output.
Normally, I could use these commands separately:
grep "error" Jog-txt
and then use:
head
My tool combines these operations so that I can search for a word and limit the results to the first few matches.

How to Run the Tool
First, clone or download this repository from GitHub.
Open a terminal and navigate to the project folder:
 cd fancy-command
Make the script executable:
chmed +x fancy.sh
Then run the tool by providing a search word, the file name, and the number of results to display:
./fancy.sh error 1og.txt 5
For example, if 1og.txt contains:
System started
User Logged in
error: connection failed
File created 
error: network unavailable
User logged out 
error: permission denied
Backup completed
Running:
./fancy.sh error log.txt 2
would display the first two matching lines:
error: connection failed error: network unavailable

Example
The basic idea behind my tool is:
grep "error" log.txt | head -n 2
Instead of typing both commands, my script combines them into one command.


Section 2 - AI-Assisted Programming

What I Asked AI

I used AI to help me understand Linux commands and how to create a simple command-line tool.
Some of the questions 1 asked AI included:
• What does the grep command do?
• What does the head command do?
• How can I combine two Linux commands?
• How can I create a Bash script that accepts command-line arguments?
• How can I make a Bash script executable?
• How can I test my command in the terminal?
• How can I upload my code to GitHub?

Where AI Helped
AI helped me understand the purpose and syntax of grep and head. It also helped me understand how the pipe (1) works in Linux.
For example:
grep "error" log-txt | head -n 5
Al explained that the output from grep is passed to head, which then displays only the first five matching lines.
Al also helped me understand basic Git commands such as:

git init 
git add .
git commit -m "Initial commit"
git branch -M main 
git remote add origin < repository-url>
git push -u origin main

Where 1 Had to Think Independently
I had to decide what kind of "fancy" command I wanted to create. I chose to combine grep and head because I understood what each command does and thought combining them would be useful for searching log files.
I also had to create and test my own text file, choose the search terms, run the command in the terminal, and verify that the output was correct.
I had to make sure the script accepted the correct arguments and that the commands worked together as expected.

What AI Got Wrong or Missed
AI sometimes provided commands without considering the exact folder or file names on my computer. I had to change the commands to match my own environment.
I also learned that simply copying a command from AI does not guarantee that it will work. I had to test the commands in the terminal, read the error messages, and make corrections when necessary.
For example, if the file name or path was incorrect, the command would not work even though the command itself was valid.

Conclusion
AI was useful for learning Linux commands, Bash scripting, and Git. However, I still had to understand the commands, test the code, troubleshoot errors, and make decisions about how to build my tool.







