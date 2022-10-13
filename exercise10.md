# Exercise 10 - Understanding Commits

1. Look at your commit log

        git log --oneline

2. Choose a commit hash

3. See what type of object that hash names

        git cat-file -t <hash>
        commit

4. Examine the contents of that commit closely

        git cat-file -p <hash>
        C:\cisw17\my_repository>git cat-file -p d265096
        tree 63f200aba7fa91b8f286d1db309941ff47b2682c
        parent 359dfe189cd477c000fcfdb15f68f0b3a1ec303f
        author Stefania Castaneda <steffcastaneda18@gmail.com> 1665693109 -0700
        committer Stefania Castaneda <steffcastaneda18@gmail.com> 1665693109 -0700

        Added vegetables to the list

5. Find the parent's hash in the commit log

        parent 359dfe189cd477c000fcfdb15f68f0b3a1ec303f

6. Look at the contents of the tree

        git cat-file -p <hash>
        C:\cisw17\my_repository>git cat-file -p 63f200
        040000 tree fa435e77db6e006f3d1c9ed56ccdf8ab91539f4f    equipment
        100644 blob a3c4ec315cfd789a7d3b0130857d353e9846bd4b    fruits.txt
        100644 blob e922e6074fe84462c6b000170e0b34b0af92015d    vegetables.txt

7. Examine the contents of one of the blobs

        C:\cisw17\my_repository>git cat-file -p a3c4ec315
        apple
        banana
        tomato
        blueberry
        strawberry
        pineapple

8. What type of object does the parent hash represent?

        git cat-file -t <hash>
        commit

9. Examine the contents of the parent and its tree


10. Do the trees you looked at have any matching hashes listed?

        Yes, all list the contents within their respective folders
