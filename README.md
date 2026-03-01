# Linux-Fundamentals-Part-1-Write-Up

## INTRODUCTION
This write-up describes the hardest challenge I encountered in the Linux Fundamentals Part 1 room on TryHackMe.

First, in this lab I practiced basic Linux commands:
- echo: print text in the terminal
- whoami: display the current user
- ls (list): list directory contents
- cd (change directory)
- pwd (print working directory)
- cat (concatenate): display file contents

These commands helped me navigate directories and read files in the terminal more confidently.

## BASIC COMMANDS EXAMPLES
### Echo
<img width="607" height="85" alt="echo png" src="https://github.com/user-attachments/assets/00fc4647-f82a-4a2e-ad52-50b1dc87af08" />

### Whoami
<img width="353" height="71" alt="whoami png" src="https://github.com/user-attachments/assets/4740fa84-15e2-4dc4-bd35-3d35722ef48f" />

### Ls
<img width="623" height="86" alt="ls png" src="https://github.com/user-attachments/assets/b2586f11-da96-4598-aa94-7cb5ef5b359c" />

### Cat
<img width="761" height="66" alt="cat png" src="https://github.com/user-attachments/assets/2313d660-33ee-4e37-a483-e3cc3d7687b1" />

## HARDEST CHALLENGE
The hardest challenge for me was finding a specific word inside a log file using the **"grep"** command.

At first, I failed because I didn't fully understand the syntax of the command and I misunderstood what I needed to search for. I initially tried:
- `grep *.THM access.log`
- `grep "*.THM" access.log`

After reviewing the syntax again, I realized that I needed to search for the text itself, so I used:
`grep "THM" access.log`

This command returned the flag in the format **THM{---}**.

### Grep
<img width="936" height="132" alt="grep png" src="https://github.com/user-attachments/assets/4c810844-2fba-439a-9b97-dd828ccb1f37" />


It is also possible to use the "-R" option to search recursively through directories.

## ADDITIONAL COMMANDS AND OPERATORS LEARNED

Other important commands I learned were "find" and "wc".

The "find" command is an efficient way to search for files because it automates the search process when you know the file name or at least the file type, for example ".txt" files.

The "wc" command can be used to count entries or lines in a file, which helps decide whether it is better to read the file with "cat" or filter the content using "grep".

I also learned about operators such as:

- `&` to run commands in the background  
- `&&` to execute commands sequentially  
- `>` to overwrite output into a file  
- `>>` to append output into a file

### Find
<img width="608" height="68" alt="find png" src="https://github.com/user-attachments/assets/d501ac5f-c26b-476d-ba42-8d56e21aad39" />

### wc
<img width="549" height="63" alt="wc png" src="https://github.com/user-attachments/assets/23a2b91c-43f9-4044-a9f6-ec2c3b034c65" />

### Operators
<img width="727" height="304" alt="operators png" src="https://github.com/user-attachments/assets/51a09fed-c49e-475d-86e2-d22ede08e82e" />

## CONCLUSIONS
From this room I learned:

- Basic Linux commands
- Correct syntax and use of the "grep" command
- How to search for files efficiently using the "find" command
- How to search efficiently in the terminal
- The importance of correct command syntax
