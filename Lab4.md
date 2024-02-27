__Part 1: Vim__
- *Step 4*
  - I was tasked to log into our `ieng6` account. Since I logged into my `ieng6` account previously from trying to perfect the efficiency, I was about to use the up arrow key to when I used that command last.
  - ![Image](lab4step4.png)
  - When in the terminal, I pressed the up arrow key once and it brought up the last command I used outside of my `ieng6` account, which was the `ssh jung@ieng6.ucsd.edu` command.
  - Keys pressed: `<up> <enter>` . The `ssh jung@ieng6.ucsd.edu` command was 1 up in the command history.
 
- *Step 5*
  - I was tasked to clone the forked repository into my `ieng6` account. In order to make the process more efficient, I copied the protected SSH Key for my forked repository on my github page (git@github.com:jeffungg/lab7.git). Then, in my terminal, I typed `git clo<tab> <Command-V> <enter>`. To make the process more efficient, I typed `git clo` and then tab to let it finish it to `clone`. Pressing Command-V lets me pastes the copied SSH Key into the command line instead of manually typing it out.
  - ![Image](lab4step5.png)
  - Keys pressed: `<git clo> <tab> <Command-V> <enter>` . Forked repository is now cloned to my `ieng6` account.

- *Step 6*
  - I was tasked to run the JUnit tests provided in the `lab7` repository and see that they fail. During the lab, when trying to find the best way to compile and run properly, I was able to put both `javac` and `java` commands into one line. Because there were a lot of trial and errors when finding an effective way to do so, using the up arrow key will take too much time. So I used the `<Ctrl-R>` command. Using this command let me search through the command history by searching for the `javac` command that I wrote earlier. Because I was able to figure out how to run both `javac` and `java` commands with one line, that meant that I only needed to use the `<Ctrl-R>` command once instead of twice, improving the efficiency.
  - ![Image](lab4step6.png)
  - Keys pressed: `<Ctrl-R> javac <enter>` . Ran the tests and showed 1 failure.
  - ![Image](lab4step6part2.png)

- *Step 7*
  - I was tasked to edit the code file to fix the failure when running the Junit tests. During the lab, I was trying any way to edit the code in a single command line without having to go into the file with `vim` and using the arrow keys to manually fix the typo. After some discussions with my labmates, we were able to improve our technique ten fold. Because I ran many commands and doing trail and error, using the up arrow keys to find the right editing command would take some time. So again, I rely on the `<Ctrl-R>` command. Then I use the `vim` command which goes into the specified file `ListExamples.java`, goes to the line specified (44), then replaces the typo(index1) with the correct one(index2).
  - ![Image](lab4step7.png)
  - Keys pressed: `<Ctrl-R> vim <enter>` . Edited the typo in ListExamples.java file.
 
- *Step 8*
  - I was tasked to run the Junit tests again but now showing that they pass. Because I had recently ran the tests. I was able to easily use the up arrow keys to access the command I used.
  - ![Image](lab4step8.png)
  - Keys pressed: `<up> <up> <up> <up> <enter>` . Ran the Junit tests
 
- *Step 9*
  - I was tasked to commit and push the code changes to my github account. I concluded that there were no easier way than just typing the commands out itself. Obviously I could've used the up arrow keys or the `<Crtl-R>` command but I'm going to assume this is the first time. `git add . ` adds any modified files to `git`'s staging area. `git commit -m "Update ListExamples.java"` commits those modified files into their own place then `git push` uploads those modified files into my remote github repository.
  - ![Image](lab4step9.png)
  - ![Image](lab4step9part2.png)
  - Key pressed: `git add . <enter> ` `git commit -m "Update ListExamples.java" <enter> ` `git push <enter> ` . 
