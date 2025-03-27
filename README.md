# Workshop on Command Line Skills for Humanists and Social Scientists

Hello world! We from the Digital Media, Arts, and Technology Program at Penn State Behrend are here to present a hands-on workshop to familiarize ourselves with command line skills. Learning to access computers at command line is both timely and a historic look backward to a time in the 1980s and 90s when the graphical user interface was new and unfamiliar for use in personal computers. The workshop will give everyone a tour of things we can see and explore at a touch with the command line in a cross-platform compatible context available for Windows, Mac, and Linux users. We will circulate instructions in advance to work with the free and open source Git Bash Shell to explore common powerful command line skills available to all of us who work with computers. We'll discuss and reflect on the history and ongoing significance of command line skills for technological literacy in the humanities and social sciences—especially during the age of AI.

### *Learning Objectives*
* Learn basic command line skills: how to navigate, organize, search files
without the graphical user interface;
* Gain historical perspective on the command line interface in the evolution of
computing “over the decades”; 
* Learn about cross-platform compatibility working with the Git Bash shell in
the context of Mac, Linux (posix) systems vs. Windows;
* Discuss the importance of command line skills for projects in humanities and
social sciences.

## Agenda: 

* (5 min) Introductions (Dr. B and DIGIT 496 students)
* (5 min) Brief history & what is command line? Command line vs. GUI
* (3 min) Windows vs. Mac (Using Git Bash Shell on Windows vs MacOS Terminal)
* (2 min) What is your "home" directory?
* (15 min) Basic command line navigation / explore sample directories & text files
* 10 min: Grepping, word counts, and piping to output files.
* (5 min) If time, Git demo.
* (5 min) Question-time / attendees can clone/pull GitHub repo

## Notes:
* Open your shell. :-) 
* Right-click on a directory and open your shell (Git Bash for Windows or Terminal for the Posix (Mac/Linux) machines).
* [Download our GitHub as a zipped directory](https://github.com/newtfire/command-line-workshop/archive/refs/tags/1.0.zip) and unzip it and save it somewhere useful: Downloads or Desktop. 
*  Navigate there in your shell. (Or right-click in your GUI file manager and open your shell.

### Git Installation Instructions
  * **Windows:**
    * Install: [https://git-scm.com/download/win](https://git-scm.com/download/win) (probably choose the 64-bit download)
    * How to tell whether you have 32-bit or 64-bit? [https://support.microsoft.com/en-us/windows/which-version-of-windows-operating-system-am-i-running-628bec99-476a-2c13-5296-9dd081cdd808](https://support.microsoft.com/en-us/windows/which-version-of-windows-operating-system-am-i-running-628bec99-476a-2c13-5296-9dd081cdd808)
  * **Mac:**
    * Open your Terminal app (Launchpad: look for Terminal):
    * Type in: `git --version`
    * Follow the instructions to install git

#### Basic Command Line Navigation
* `pwd` from where you are
* `ls` to "look see"
* `cd` down into a directory
* `cd` up with `cd ..`
* `ls -lh` and `ls -lisa` 
* `cat filename.extension` to view an existing file

#### More commands for Making/Changing Directories/Files
* `mkdir directoryName` make a directory
* `vi` and `nano`: create and store a file
* `rm` and `rm -r` (but please be careful!)
* `mv` vs `cp`:
     * `mv sourcePath targetDirectory` (can be used to rename a file, too)
     *  `cp sourcePath targetPath`: `cp myDirectory/file.txt ..` moves up to the parent directory.
     *  What's the difference between `cp` and `mv`?

* **Your Turn**:
    * Can you make a directory and/or file, and move the file to a new location? 


#### More commands to explore/study Directories and Files
* `wc filename.extension` for word count. (Try on one of our files.)
* `grep` (stands for "global regular expression print" (as in print to console). 
    * Grep over a single file for the pattern "rest" (USE THE TAB TO AUTOCOMPLETE THE FILENAME IN THIS): `grep "free*" lotr/01-The-Fellowship-Of-The-Ring.txt --color=always`
    * Pipe the results to a word count (the number of matches) with `wc`: `grep "free*" lotr/01-The-Fellowship-Of-The-Ring.txt | wc -l`
    * Grep over a file directory for the same pattern: `grep -r "free*" lotr/` (Note: color settings should hold in the same shell session.)
* **Your turn**: Find out how often "free*" (or a word or word-stem of your choice) appears in political speeches by one or two presidents in our collections. (Use `ls` to explore our command-line-workshop files).
    * **Pipe the results** to a file that you save: `grep -r "free*" lotr > mygrepResults.txt`
    * Use `ls` to look for your file. Use nano or vim to open it. CTRL + X to escape the view window.

* More complicated things can be done with shell-scripting (multiple lines, for loops) or, better yet, Python. But you need basic shell commands for a start!

##### Optional Git/Github demonstration (if we have time)
* Dannika and Caleb demonstrating pushing and pulling new files to the command-line-workshop repo.
  
## For Review and Reference:
* [Our interactive web slide-tutorial](https://slides.com/elisabeshero-bondar/shell-git-nav/)
* [Geeks for Geeks: Basic Shell Commands](https://www.geeksforgeeks.org/basic-shell-commands-in-linux/)
* [Geeks for Geeks: Basic Linux Commands for day to day life](https://www.geeksforgeeks.org/basic-linux-commands-day-day-life/)
* [Educative: Bash Cheat Sheet](https://www.educative.io/blog/bash-shell-command-cheat-sheet)

  


  

