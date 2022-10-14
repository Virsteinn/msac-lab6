# Exercise 7 - More than one changed file

1. Ensure you have a clean working directory

        git status

2. Edit one of your `fruits.txt`, add a few items

        blueberry
        strawberry
        etc.

3. Edit `appliances.txt` and add a few items

        dishwasher
        dryer
        etc.

4. Look at git status, paste the output here

        git status

        $ git status
        On branch master
        Changes not staged for commit:
          (use "git add <file>..." to update what will be committed)
          (use "git restore <file>..." to discard changes in working directory)
                modified:   equipment/appliances.txt
                modified:   fruits.txt

        no changes added to commit (use "git add" and/or "git commit -a")

5. Can you commit both of the changed files in a single commit?

        Yes.

6. After you do so, check that you have a clean working directory by running `git status`, and pasting the output here

        $ git status
        On branch master
        nothing to commit, working tree clean

7. Create a new file `equipment/furniture.txt`. Add content to both `vegetables.txt` and `furniture.txt`

8. How can you commit just one of the changed files?

        Stage one with a `git add` command, and then run a `git commit` command. The unstaged file will not be committed.

9. Check your `git status`

10. What does red text mean in the output of `git status`?

        Red text indicates the files in the output, new or modified, have yet to be staged. These files will not be committed on a `git commit` command.

11. What does green text mean in the output of `git status`?

        Green text indicates the files in the output, new or modified, are staged, and will be committed on a `git commit` command.

12. How can you make a single file show in both red and green in the output of `git status`?

        First, stage the changes you have already made. Then, make more changes, and run a `git status` command. The changes you had already made and staged will show as a green version of the file, while those made subsequent to the staging will show as a red version.