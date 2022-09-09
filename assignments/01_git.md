# Git/GitHub Assignment

* **INDIVIDUAL ASSIGNMENT**
* **Due date**: Sept-13th 11:59PM
* **Value**: 100 points counted towards Homework category.

## Description
This assignment is composed of two parts. 
- [Part 1](#Part-1-Dealing-with-git) consists of executing a sequence of commands and giving explanations about the commands you have to run. For each question, please provide appropriate explanation and/or the details requested.

- [Part 2](#Part-2-Using-GitHub) consists of creating a Markdown file on a fork of this course and creating a pull request towards this repo.

### Part 1: Dealing with git

To conduct this, you will have to download [handson.zip](handson.zip) and unzip it in your local machine. **Note:** handson folder is a git repository.

Then, follow these steps:

**On GitHub:**
1. Create a new repository under your GitHub account called *INF502*;
2. Create a file called *"Assignment1.md"*;
3. Copy the questions from this section and paste in your *"Assignment1.md"* file (tip: to copy the questions, click on *"Raw"* at the right-top of this file; this will show you the markdown source);
4. For each empty grey box, please provide an answer to the questions below.
5. Invite me to see your new repository. This will allow you to keep a private repository that only you and me will be able to see.

Your submission is complete when you complete the *Assigment1.md* file with your answers and invite me to your repo.

**On your local machine:** Using the command line, find and access the "handson/" directory (if you didn't download and unzip the file, go back to the beginning of Part 1's instructions). Then, answer the following questions (on your *Assigment1.md* file):

1. List all the branches in this repository and, for each branch, list the commits.

    - Use `git branch` to list the branches in this repository.
    - Use `git checkout` to explore each branch.
    - Use `git log --decorate` to explore the structure of commits.

```
1.git branch 
* main 
2.git checkout master
Switched to a new branch 'master'
3.git log --decorate
commit 42d52158a1a14c8c211b89f0aefcd077267a573b (HEAD -> main, origin/master, origin/main, master)
Author: Sasi8333 <98135425+Sasi8333@users.noreply.github.com>
Date:   Wed Sep 7 21:10:30 2022 -0700

    added the data

commit 99c49f91c50e6f42203d95d36e5cd8610fee3fb9
Author: Sasi8333 <98135425+Sasi8333@users.noreply.github.com>
Date:   Wed Sep 7 14:36:46 2022 -0700

    file Created

```

2. Try `git log --graph --all` to see the commit tree. Paste the result here and write a paragraph to provide an interpretation of what you found.
```
 git log --graph --all
* commit 42d52158a1a14c8c211b89f0aefcd077267a573b (HEAD -> master, origin/master, origin/main, main)
| Author: Sasi8333 <98135425+Sasi8333@users.noreply.github.com>
| Date:   Wed Sep 7 21:10:30 2022 -0700
|
|     added the data
|
* commit 99c49f91c50e6f42203d95d36e5cd8610fee3fb9
  Author: Sasi8333 <98135425+Sasi8333@users.noreply.github.com>
  Date:   Wed Sep 7 14:36:46 2022 -0700

      file Created



git log --graph -all command display the all the commits history nad we can see tex based history of all the commits include author name and date as well as commit message.

we can see graphical representation of the commits from the left side lines.

```

3. Use `git diff BRANCH_NAME` to view the differences from a branch and the current branch. Summarize the difference from master to the other branch.

```
git diff master
diff --git a/Assignment1.md b/Assignment1.md
index 2455c8b..cbfee24 100644
--- a/Assignment1.md
+++ b/Assignment1.md
@@ -34,8 +34,6 @@ Your submission is complete when you complete the *Assigment1.md* file with your
     - Use `git log --decorate` to explore the structure of commits.

 ```
-1.$ git branch
-* main


 ```
diff --git a/sample b/sample
deleted file mode 100644
index e69de29..0000000


git diff command will disply the differences bitween two branches.

for exmple we observe above  output it showing the difference btiween the main and master branch.



```

4. Write a command sequence to merge the non-master branch into `master`.

```
First we run git checkout master to change the active branch back to the master branch. Then we run the command git merge new-branch to merge the new feature/task into the master branch.


git merge new-branch

```


5. Write a command (or sequence) to (i) create a new branch called `math` (from the `master`) and (ii) change to this branch.

```


```
   
6. Edit B.py adding the following source code below the content you have there.
```
print 'I know math, look:'
print 2+2
```

7. Write a command (or sequence) to commit your changes.
```


```

8. Change back to the `master` branch and change B.py adding the following source code (commit your change to `master`):
```
print 'hello world!'
```

9. Write a command sequence to merge the `math` branch into `master` and describe what happened.
```


```
   
10. Write a set of commands to abort the merge.
```


```
   
11. Now repeat item 9, but proceed with the manual merge (editing B.py). All implemented methods are needed. Explain your procedure.
```


```

12. Write a command (or set of commands) to proceed with the merge and make `master` branch up-to-date.
```


```

13. Complete Part 2. Then, come back here and answer the following:
Report your experience of submitting the Part 2. Please, include the steps you followed, the commands you used, and the hurdles you faced (within the file you created for the **Part 1**).
```


```

### Part 2: Using GitHub

The goal of this assignment is to put you in touch with the fork-pull request process, with an extra of dealing a little bit with Markdown. To learn more about Markdown [click here](https://guides.github.com/features/mastering-markdown/).

To complete this submission, follow these steps:

1. Fork the course repository (available [here](https://github.com/chavesana/INF502-Fall22)).

2. Into the students folder, create a markdown file called LASTNAME_FIRSTNAME.md (please change LASTNAME_FIRSTNAME for your actual last and first names). 

3. Use markdown to write a report of the last paper you've read. You can structure your markdown the way you want, but the following information must be there:
- Title
- Venue (journal name/conference)
- Number of pages
- Three outcomes of the paper
- Link to the paper online

4. Commit your file and push to your own GitHub repository (INF502).

5. Create a pull request to the course repository. Your pull request needs to appear [here](https://github.com/chavesana/INF502-Fall22/pulls).

6. Go back to Part 1 and answer the question 13 based on your experience in solving Part 2.

Your Part 2 submission is complete when your pull request is listed in the link above.
