GIT:
---
git is a distributed version control system here every one will have a local repository. 
All the local repository has  all of the information that a remote repository has based on the last time that we sync those two together. 
We can also have option that for central reomte repesitory. 
If we don't have access to the remote repository then we can still view every single change that's been made to that repository since it was created.
so almost every developer(working on it) has an entire backup of the repository. 
In the worst case if something happening to the remote repository every developer has a copy of that same repository on their machine so that's why it is called as a distribution version control system.


how to do change to a file and update to existing file which is in github

step1:
-----
run the maste and say ur are working on some file "readme.txt" 
$git branch readme.txt

step2:
-----
switch the branch to readme
$git checkout readme.txt

now your are working on readme branch 
now do changes what ever you want do in readme.txt file

step3:
-----
$git status 

you can see that "readme.txt" hasbeen modified

step4:
-----
To add that modification to the file. we need to add that to our staging directory.

$git add -A

step5:
-----
Now we want to commit what changes we have done. commit message must be more detail that what we have done to that file.

$git commit -m "[need to write what modification you have done]"
ex:
$git commit -m "added new subtraction function to the code" 

step6:
-----
now we need to push that changed file to our remote repository
$git push -u origin readme.txt

NOTE:we need to git our github login details

step7:
-----
if all the test ran well then we can merge this with our master/main. we can checkout out master/main branch.

$git checkout master/main 

means now again we switching back to our master/main brach. which we have changed in "step2" (which we have switched from master/main to readme branch)

step8:
-----
We need to pull master/main branch because we want to pull in all the changes that hvae been made.

$git pull origin master/main

Now we have pull the all the changes.

step9:
-----
now we can merge the "readme" branch with master/main

$git merge readme.txt 

step10:
------
Now we can push those changes 

$git push origin master/main.


Now go to github you can check the file which you have modify

refernce:
--------

https://dzone.com/articles/top-20-git-commands-with-examples

https://www.youtube.com/watch?v=HVsySz-h9r4

