# QuickGit
Two short bash functions I wrote to speed up terminal navigation and updating git.
There are two main methods here...."webserver" and "updaterepo". 
They will need to be in your user .bash_profile file to be used. 

# NOTE: These instructions/scripts are for a MacOS environment. I've written slightly detailed instructions for users who may be less knowledgeable of Unix based terminal usage. Rudimentary knowledge of terminal use is recommended.

  1.) Open Terminal
  2.) type: "cd /Users/myUser" where 'myUser' is your system profile name. Hit return. 
  3.) type: "ls -a". Hit return 
  4.) vi .bash_profile and hit the "i" key (insert mode)
  5.) copy and paste the bash functions (QuickGit.txt) into this file
  7.) Hit the esc key, then type ":wq!" and hit return
  6.) Restart Terminal to use these functions

# <-- WEBSERVER -->
This is a simple function that takes you to your local webserver (XAMPP, MAMP, etc) no matter what directory you are in. 
You can run this with or without a passed parameter...

  webserver
  
     OR
     
  webserver myrepofolder
  
 (Running with a parameter will take you directly to the specific repo folder you want.)

# <-- UPDATEREPO -->
This function will update your repository with one simple step rather than the typical "git dance" (git add, git commit, git push). This function is best to use when you are simply updating to the master branch of a project.

To use this function, you must currently be in a git directory (if not, you should receive an alert that you are not in a directory with a git repository). 

While in a directory with a git repo...simply type the command:
  "updateRepo 'This is my commit message'" 

Hit enter.
(If you do not provide a commit message or as a string you will receive an error)

