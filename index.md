# Lab Report 4

### Introduction:
In this lab report, the steps on how to successfully log into an SSH server and download, edit, and upload changes to a programming project all from the command line are detailed. For each step below, there is a description along with a screenshot and a list of exactly which keys were pressed. Bash, vim, and git (from the command line) are the main tools used in this lab report.

### Step 4: Log into ieng6

In this step, the user logs into ieng6 using the ssh command and the user’s ieng6 username.

![!Image1](screenshot11.png)

**Keys Pressed: `"ssh cs15lsp23bw@ieng6.ucsd.edu"`, `<Enter> (x1)`**

This step only contains one command which logs the user into the SSH server. Because of SSH keygen, no password is required.

### Step 5: Clone your fork of the repository from your Github account

In this step, the user clones their fork of the repository from their Github account using the git clone command.
The user then enters the downloaded folder using the "cd" command so they can perform the next steps.

![!Image1](screenshot22.png)

**Keys Pressed: `"git clone git@github.com:mberlin123/lab7.git"`, `<Enter> (x1)`, `"cd lab7"`, `<Enter> (x1)`**

The first command in this step clones the github repository to the SSH server. The second command changes the current directory to the download folder.

### Step 6: Run the tests, demonstrating that they fail

In this step, the "bash test.sh" command is run and fails due to an error in the "ListExamples.java" file.

![!Image1](screenshot13.png)

**Keys Pressed: `"bash test.sh"`, `<Enter> (x1)`**

This command runs the "test.sh" script which promptly fails due to a bug in the code.

### Step 7: Edit the code file to fix the failing test

In this step, the user fixes the bug in the code file using vim.

![!Image1](screenshot14.png)

**Keys Pressed: `"vim ListExamples.java"`, `<Enter>`, `<Down-Arrow> (x1)`, `<Right-Arrow> (x1)`, `<I> (x1)`, `<Backspace> (x1)`, `"2"`,
`<Escape> (x1)`, `":wq"`, `<Enter> (x1)`**

The commands in this step are the most complicated due to the extensive nature of the Vim command system. The first command opens Vim in Normal mode. Due to the arrow cursor being positioned close to the bug in the code, only a "Down-Arrow" and "Right-Arrow" keypress are needed to reach the bug in the code. After, "I" is pressed to enter Insert Mode. At this point, "Backspace" and "2" are pressed to fix the bug. Finally, "Escape" is pressed to re-enter normal mode and ":wq" is pressed to save and exit Vim.

### Step 8: Run the tests, demonstrating that they now succeed

In this step, the "bash test.sh" command is run again and this time succeeds as the bug has been fixed.

![!Image1](screenshot15.png)

**Keys Pressed: `<Up> (x2)`, `<Enter> (x1)`** (To run **"bash test.sh"**)

In this step, due to the same command being run in Step 6, only two "Up-Arrow" keypresses are required (and then "Enter" of course as with all other commands".

### Step 9: Commit and push the resulting change to your Github account

In the final step, the changes are uploaded to the user's github repository. 

![!Image1](screenshotfinal.png)

**Keys Pressed: `"git add ListExamples.java"`, `<Enter> (x1)` `"git commit -m "Fixed ListExamples.java"`, `<Enter> (x1)`, `"git push"`, `<Enter> (x1)`**

The first command adds "ListExamples.java" to the tracked files. The changes to the file are then saved with the second command. Finally, the changes are uploaded to the github repository with the final command.
