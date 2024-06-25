# PLP_Basic_Git_Assignment

Step 1: User@Mchael-O MINGW64 /g
            $ mkdir PLP_Basic_Git_Assignment

Step 2:  User@Mchael-O MINGW64 /g
              $ cd PLP_Basic_Git_Assignment

Step 3:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment
               $ git init
                Initialized empty Git repository in G:/PLP_Basic_Git_Assignment/.git/


Step 4:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
             $ git remote add origin https://github.com/WuodRose/PLP_Basic_Git_Assignment.git

Step 5:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
               $ touch hello.txt

Step : 6   User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
                 $ git status
                  On branch master
                  No commits yet
             Untracked files:
                    (use "git add <file>..." to include in what will be committed)
                         hello.txt
                        nothing added to commit but untracked files present (use "git add" to track)

Step 6:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
                $ git add -A

Step 7:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
                 $ git status
                   On branch master
                   No commits yet
           Changes to be committed:
                (use "git rm --cached <file>..." to unstage)
                 new file:   hello.txt


Step 8:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
              $ git commit -m "hello.txt with a greeting"
                [master (root-commit) 1db6709] hello.txt with a greeting
               1 file changed, 1 insertion(+)
                create mode 100644 hello.txt

Step 9:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (master)
             $   git branch -m main


Step 10:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (main)
$ gig pull --rebase
bash: gig: command not found




Step 11:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (main)
                  $ git pull --rebase origin main
                   remote: Enumerating objects: 3, done.
                  remote: Counting objects: 100% (3/3), done.
                   remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
                     Unpacking objects: 100% (3/3), 870 bytes | 66.00 KiB/s, done.
                    From https://github.com/WuodRose/PLP_Basic_Git_Assignment
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.

Step 12:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (main)
                   $ git push -u origin main
                    Enumerating objects: 4, done.
                   Counting objects: 100% (4/4), done.
                 Delta compression using up to 4 threads
                    Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 306 bytes | 306.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/WuodRose/PLP_Basic_Git_Assignment.git
   29a39c3..f50ea5c  main -> main
branch 'main' set up to track 'origin/main'.

Step 2:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (main)
                $ git status
               On branch main
              Your branch is up to date with 'origin/main'.
           nothing to commit, working tree clean

Step 13:  User@Mchael-O MINGW64 /g/PLP_Basic_Git_Assignment (main)
               $ git reflog
                 f50ea5c (HEAD -> main, origin/main) HEAD@{0}: pull --rebase origin main (finish): returning to refs/heads/main
               f50ea5c (HEAD -> main, origin/main) HEAD@{1}: pull --rebase origin main (pick): hello.txt with a greeting
               29a39c3 HEAD@{2}: pull --rebase origin main (start): checkout                  29a39c3bd04a1b9198f4666093b14bd068b2e31b
1db6709 HEAD@{3}: Branch: renamed refs/heads/master to refs/heads/main
1db6709 HEAD@{5}: commit (initial): hello.txt with a greeting


