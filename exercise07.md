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
        C:\cisw17\my_repository>git status
        On branch master
        Changes not staged for commit:
        (use "git add <file>..." to update what will be committed)
        (use "git restore <file>..." to discard changes in working directory)
        modified:   equipment/appliances.txt
        modified:   fruits.txt

        no changes added to commit (use "git add" and/or "git commit -a")

5. Can you commit both of the changed files in a single commit?

        Yes, you can use the line git commit -a

6. After you do so, check that you have a clean working directory by running `git status`, and pasting the output here

        C:\cisw17\my_repository>git status
        On branch master
        nothing to commit, working tree clean

7. Create a new file `equipment/furniture.txt`. Add content to both `vegetables.txt` and `furniture.txt`

8. How can you commit just one of the changed files?

        git commit filename.txt

9. Check your `git status`

10. What does red text mean in the output of `git status`?

        The file has been modified and has not been staged.

11. What does green text mean in the output of `git status`?

        The file has been modified and staged.

12. How can you make a single file show in both red and green in the output of `git status`?

        You can make a single file show in both red and green by adding a modified file to staging and then editing the file again without commiting the original changes.

