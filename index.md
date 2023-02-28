Dara Arbab
Lab Report 4

Step 1 for this lab was to log into the ieng6 server.

I did this by typing the following:

ssh cs15lwi23axd@ieng6.ucsd.edu

A password is not needed to log in as I already have an ssh key set up for the server.

![step1.png](/step1.png)

Step 2 for this lab is to use the git clone command to clone the lab repository from my github into the server.

I did this by first copying the git address for the repo, then, typing the following:

git clone <COMMAND> <V>
-- command v pasted the following: git@github.com:1821858/lab7.git
  
![step2.png](/step2.png)

Step 3 for this lab is to run the junit tests proving that the code fails and has a bug.
  
I did this by typing the following:
  
javac -cp "./lib/hamcrest-core-1.3.jar:./lib/junit-4.13.2.jar" T<TAB> L<TAB>

This placed the following in the command line:
  
javac -cp "./lib/hamcrest-core-1.3.jar:./lib/junit-4.13.2.jar" TestListExamples.java ListExamples.java
  
Running the command gave this failure output:
  
![step4.png](/step4.png)

Step 4 for this lab is to edit the file ListExamples.java to correct the bug.
  
I did this by using nano to open and navigate to the bug and fix it. I did this by typing the following:
  
nano ListExamples.java
  
Once the file was open I used the arrow keys to navigate to "List1" in the last while loop, and change it to "List2".
This resolves the bug, and we can save, recompile, and rerun the tests, seen here passing.
  
![step5.png](/step5.png)
  
Now that our bug has been resolved and our code passes the tests, we can commit to this change.
  
We do this by using the git add, git commit, and git push commands.
  
Step 6 is to add the new files.
  
We do this with the following command:
  
git add --all
  
Step 7 is to commit the changes
  
git commit -m Updated
  
And step 8 is to push this to our git repository
  
git push
  
These steps are shown here
  
![step6.png](/step6.png)
