# Exercise 8 - Viewing changes before committing

1. Ensure your working directory is clean

2. Add text to any one of your files

3. Delete different text from another of your files

4. Look at `git status`

5. View all the changes you've made

        git diff

6. Does the following command return anything?

        git diff --staged

        Nope.

7. Add one of your changed files to the index

        git add <changed file>

8. What do these commands show?

        git diff

        $ git diff
        diff --git a/vegetables.txt b/vegetables.txt
        index 9ac7af5..d1a7482 100644
        --- a/vegetables.txt
        +++ b/vegetables.txt
        @@ -1,5 +1,4 @@
        potato
        broccoli
        eggplant (please God no)
        -brussels sprout (I hate the person that made this list)
        -cheese (that's not even a vegetable!)
        \ No newline at end of file
        +brussels sprout (I hate the person that made this list)
        \ No newline at end of file

        git diff --staged

        $ git diff --staged
        diff --git a/fruits.txt b/fruits.txt
        index df1bc08..3632ceb 100644
        --- a/fruits.txt
        +++ b/fruits.txt
        @@ -1,6 +1,7 @@
        apple
        banana
        tomato
        +jackfruit
        durian
        minion-wait, no, that's not a fruit
        Gru-neither is he!

9. Add the other changed file to the index

        git add <other changed file>

10. What do these commands show?

        git diff

        Nothing.

        git diff --staged

        $ git diff --staged
        diff --git a/fruits.txt b/fruits.txt
        index df1bc08..3632ceb 100644
        --- a/fruits.txt
        +++ b/fruits.txt
        @@ -1,6 +1,7 @@
        apple
        banana
        tomato
        +jackfruit
        durian
        minion-wait, no, that's not a fruit
        Gru-neither is he!
        diff --git a/vegetables.txt b/vegetables.txt
        index 9ac7af5..d1a7482 100644
        --- a/vegetables.txt
        +++ b/vegetables.txt
        @@ -1,5 +1,4 @@
        potato
        broccoli
        eggplant (please God no)
        -brussels sprout (I hate the person that made this list)
        -cheese (that's not even a vegetable!)
        \ No newline at end of file

11. Commit the changes

12. Check that your working directory is clean

13. Create a new file named `clothing.txt`

14. Does the new untracked file show up in git diff?

        git diff

        No.

15. Add and commit the new file
