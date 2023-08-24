![Tec logo](/images/Tec-logo.jpg)

# **What is Github and what I've done until now**

##Basics
*Github* is a platform used for collaborative coding and it lets you and others work from anywhere. :computer:
![Github logo](/images/GitHub-logo-2-imagen.jpg)


##What I've learn
####**Week 1**
#####Day 1
A brief introduction to what *Github* and *GitBash* are and how to set up the basics such as, creating an account, dowloading *GitBash*, and changing the necessary settings in order to formally start using the platforms.

In order to being using the platforms, we learned the basic codes for *GitBash*
> **clear** (clear screen)
    > **pwd** (print working directory)
    > **ls** (list)
    > **ls -A** (list all)
    > **cd** (change directory)
     **push**
     **pull**

What are push and pull?
Push and pull are codes that allow the user to save and extract information in the *Github* and your computer.
With this information in mind, we created a README document in order to start coding information to the page and a repository page in *Github* in order to upload and save documents.

#####Day 2
After learning the basic codes, we started modifying a document in order to change its appearance and information in it. The modified document was saved by using the **commit** code uploading it to *Github*.
The formats for titles (#text) and subtitles (##text) were taught. We kept practicing the basic codes in order to get familiar with them, more specific the push pull codes.

#####Day 3
We dowloaded a program to keep coding and visualize the changes made in the README document at the same time. *Visual Studio Code* is "a streamlined code editor with support for development operations like debugging, task running, and version control."
In such program, we dowloaded the *Mardown preview* in order to be able to visualize the changes made in real time and how it is going to be seen. We also learned how to add images, links, and emojis to the README document using a cheat sheet from the [Markdown Guide](https://www.markdownguide.org).
With the information learned form the past 3 days, we were able to modify the README document to our preference, allowing us to get a step closer to final objective of becoming an engineer in computer science. :computer:

![ITC TEC](/images/page_1.webp)

####Week 2
#####Day 4
We began to learn how various people can work at the same time in one project. 
It's not recommended to work in the main branch and make the changes in different branches (*Development* and *Testing*), each with its respective function. The *development* branch is mostly used to make changes that you want to make in the main branch, the *testing* branch is used to test the changes made in the *development* branch, and finally, if the testing process was successful, you upload the changes directly to the main branch.
That is the recommended process, but we are going to skip the *testing* branch and only focus on the *development* and main branch.
We created an *Operations* python branch by using the following code:
> **git checkout -b Operations**

After creating the branch and saving the changes, we got back to the main branch by using the following code
> **git checkout main** and **git checkout "name"**, name is the name of the branch wanting to move to.

After adding and pushing the changes to the Operations branch, it is time to push the changes into the main branch. In order to do that a simple click is all that is needed.
A click on a green button that says *pull request*.

A new code was introduced that gets back all the changes made and deletes the remote branches that are not being used.
>**git fetch --prune**

And after using **git pull**, the branch that is not used is fully deleted.

#####Day 5
We officially began the process to work in teams. In order to do that, we had to make a collaboratory repository through settings.
After sending or accepting the request, depends on your role, clone the repository into your files with *git clone*.
Individually, we created a new branch with our student number and modified the document in it. After add, commit, and push process, the supervisor has to merge the pushed changes through the pull requests done by the other teammates.
Due to the various changes made, a problem is going to happen when trying to merge. It is the supervisor's job to solve the problems when trying to merge.
After solving the problems, the team members have to *git pull* the information to their computer.
With all the previously done process in mind, we had to create a python document each adding an equation to the document through a separate branch, and the supervisor merging them all together.

#####Day 6
We learned how to do the merging process directly from our computers instead of using **Github**. In order to do that, the team members have to make a change in their respective branches and create a pull request to the supervisor. The following code is going to be used by the supervisor in the terminal.
>**git fetch --all**
**git pull**

After using *git pull*, it should say that it is already up to date. If it does, the next step is to write **git merge origin "name of the branch"** If there are no conflicts, the supervisor has to push the changes to the origin main with **git push -u origin main**
It is also necessary to delete the branch the change was made on, in order to do this we have to use the following code. **git push origing -d "name of the branch"**
