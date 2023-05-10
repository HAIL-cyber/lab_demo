# lab_demo
this repo will contain demonstration about git branches

# step 1 : create local repository [demo] -> cd demo
# step 2 : initialiez the local repostiroy as git repository -> git init
# step 3 : clone the remote repository to local repository -> git clone [remote:url]
# step 4 : create the required file structure 
    master -> sub
                \___lab1
                |___lab2
                |___lab3
    -> git branch sub
    -> git branch lab1
    -> git branch lab2
    -> git branch lab3

# step 5 : switch to lab1 branch and create the required files
    -> git checkout lab1
    -> touch script1.sh script2.sh
    -> git add -A
    -> git commit -m "message"
    -> git push -u [remote:url] lab1
# step 6 : switch to lab2 branch and create the required files
    -> git checkout lab2
    -> touch program1.py program2.py
    -> git add -A
    -> git commit -m "message"
    -> git push -u [remote:url] lab2
# step 7 : switch to lab3 branch and create the required files
    -> git checkout lab3
    -> touch file1.txt file2.txt
    -> git add -A
    -> git commit -m "message"
    -> git push -u [remote:url] lab3
# step 8 : switch to sub branch and merge the required branches
    -> git merge lab1 lab2 lab3
    -> git add -A
    -> git commit -m "message"
    -> git push -u [remote:url] sub
