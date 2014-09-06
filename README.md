## Assignment 01

***Objective.*** The purpose of this assignment is to help you grow in your familiarity with git, github, and R markdown. What you do in this workflow will be needed to perform and submit your assignments. In addition to figuring out how to the technicalities of working on your assignments, it will help you to develop the skills you need to carry out two significant parts of performing reproducible research. This assignment is to be completed by the end of ***Friday, September 12***.

1\. In class I have mentioned the Software Carpentry Website several times. They have some pretty good materials for teaching people how to use git and github. For the first exercise, I want you to follow their instructions on their [Version Control with Git](http://software-carpentry.org/v5/novice/git/index.html) page. These instructions involve the use of the command line git tool. This is the same tool that RStudio will use. I want you to use the command line at least once to have a better idea of what is going on under the good. To complete this exercise you will need to do items 2, 3, 4, and 6, but in the order of 6, 2, 3, and 4. After you do item 6, you will need to run the following at your prompt: `cd ~`.  
  
  ***If you are using a mac***, when you run the `nano` command and do the necessary typing, you will need to type `Control X` to save and quit. Once you hit that, you'll type `Y` and be good to go.
  
  ***If you are using a windows machine***, you will need to use the gitbash tool that is available for windows. You can find this by going to the search tool in windows and typing "Git bash". Unfortunately the current version does not seem to have `nano` as part of its implementation. Instead of using `nano`, please use `notepad`. Also, the `-a` does not work with `ls` in the windows version.

When you create your `planets` repository, be sure to make it public so that I can see it.


2\. Now we will switch to using RStudio to interact with github. The goal here is to take a text document, modify it with markdown and then submit it to the original repository as a pull request for me to evaluate. I'll be evaluating i) whether you were able to get the pull request accomplished, ii) the effort you put into making commits and having meaningful commit statments, and iii) your ability to format the document into something attractive while using as many formatting features as you can.  

You might want to pull out your copy of the R markdown cheat sheet. First, go to the [assignment repository](https://github.com/microbialinformatics/assignment01). In the upper right corner click the "Fork" button

<img src="png/OriginalRepoFork.png">

Now go to your copy of the repository and copy the repository address to the clipboard

<img src="png/MyVersionOfRepoCopy.png">

Go into RStudio and create a new project

<img src="png/RStudioFileNewProject.png">

Create it from version control

<img src="png/RStudioFromVersionControl.png">

Create it from Git

<img src="png/RStudioFromGit.png">

Enter the repository information (paste what you copied)

<img src="png/RStudioEnterCopiedInformation.png">

Now we need to chage the name of our `syllabus.txt` file to `syllabus.md`. In the lower right corner, check the box next to `syllabus.txt`

<img src="png/RStudioClickSyllabusTXT.png">

Click the `Rename` button and enter `syllabus.md` in the text field

<img src="png/RStudioRenameSylabusTXT.png">

Now look to the top of the window and you'll see `Git` written vertically. Click on that and select `Commit`

<img src="png/RStudioClickGitCommit.png">

Here you'll see the files that can be added or have been removed from the project. Click on both the `syllabus.txt` and `syllabus.md` files. Go ahead and enter a commit comment in the box to the right and click `Commit`.

<img src="png/RStudioStageNameChange.png">

Congrats - you've made your first commit! Now we need to edit our .gitignore file to ignore the files ending in Rproj since we don't want this in the repository. Go back to the lower right corner and click on the .gitignore file name to open it in a window.

<img src="png/RStudioClickGitIgnoreEdit.png">

Then add `*.Rproj` to the contents of the file and save and commit:

<img src="png/RStudioStageGitIgnoreChange.png">

Now you're ready to edit the `syllabus.md` file. I've made one edit. You need to markdown the entire syllabus file to make it look attractive with different headings, italics, bolds, hyperlinks, bullets, etc. Try to make several commit messages as you make different types of commits.

<img src="png/RStudioOpenEditSyllabus.png">
<img src="png/RStudioStageSyllabusChange.png">

When you are done editing the file and commiting the changes, click the `Push` button in the upper right corner. 

<img src="png/RStudioPush.png">

This results in you pushing your changes up to your repository in Github. Return to your repository and refresh the page. You should see that some changes have been made and that there are now several more commit messages.

<img src="png/MyNewVersionOfRepo.png">

Now you want to return to the original repository and click the `Pull Request` button

<img src="png/ReturnToOriginalRepoClickPullRequest.png">

Once there click `New Pull Request`

<img src="png/ClickNewPullRequest.png">

Then click `Compare across forks`

<img src="png/ClickCompareAcrossForks.png">

Go ahead and select your fork in the bottom option box

<img src="png/SelectYourFork.png">

Now click the green `Create pull request` button...

<img src="png/ClickCreatePullRequest.png">

Finally, enter your name and whatnot and click the green `Create pull request` button

<img src="png/EditSubmission.png">

And you're done!


3\. I would like to have a roster for the class so I can learn everyone's name along with their home department, year, and a picture. I've started one on the [course website](http://microbialinformatics.github.io/roster.html). But LeftEye (that's the pig) and I are a bit lonely. Repeating what you did in exercise 2, complete a pull request to submit your information. Please follow the formatting that I have started and include a horizontally framed selfie of yourself. The [repository for the course website](https://github.com/microbialinformatics/microbialinformatics.github.io) contains a folder called `img` for you to put your picture. As you submit your pull request I will quickly accept or reject your request so we can get everyone loaded.

