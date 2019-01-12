# FRC Robot Example using git & github

Trying to get the process down on how to setup a new robot project, put it under git control, setup a remote repo and push local changes up to github.

## Dependency 
* Download and install the *WPI/VS Code extensions*, along with the *WPILIB*. Here are the [FIRST Screensteps](http://wpilib.screenstepslive.com/s/currentCS/m/getting_started) for the setting up the 2019 Control System. There is a link to the offline installer. It's 1 gig in size, so make sure you've got the bandwidth or data limits. 

* git - You will need to have a local version of git installed so you can work with your coding team on github.
![gitdownloadpage](/images/gitdownloadpage.png)
    * [Click Here to goto the git download page](https://git-scm.com/downloads)
    * Make sure to check out the [git docs online](https://git-scm.com/docs)

* VS Code does have support for git built in, but under the market place there are maybe wonderful extensions. GitLens being one I really like. Also in the VS Code market place "Github Pull Requests".  Allowing you to submit a remote Pull Request (also know as a PR) right from the comfort of your editor.

## Process Overview
Here we will layout steps for creating a FIRST Robot project in VS Code, putting the project under git version control. Uploading it to GitHub, and setting up collaborators to help in the coding of your robot.

### VS Code and WPILIB Extension

1. In VS Code, bring up the WPILIB command pallet. 
2. Select "Create new project"
3. Enter all the basic project information. Make sure that the "Create new folder" checkbox is selected.  This will generate all the basic project files, java templates, gradle settings, etc...

You will now have a basic template robot project created.

### Creating a local git repo
4. Now using the command pallet <ctrl + shift + P>, enter git: init and you should see the option of GIT: Initialize Repository.
5.Now over on the Activity Bar, under Source Control you will have a number next to the icon.  Showing you the number of files that are un-managed and need to be added to your repository. 

![Source Control](/images/sci.png)

### Uploading to GitHub
1. Using your favorite web browser, go and login to your Github account.
2. Create a new blank repository with a meaningful name like 2019FRC5523-Robot
3. Make sure NOT to check the "Create a Readme.md" file.  All your really after here is the URL for the new repository.  Copy the URL to your clipboard.
4. Back in VS Code, bring up the command pallet <ctrl + shift + P> and enter git: push to and press enter.  
5. You will be asked for the URL to push your local git code up to.  Paste the URL that GitHub generated for you into this open field and press enter.
6. Open the command pallet once again and enter PUSH.  This should bring up a menu item of GIT: PUSH.  Selecting this, and pressing enter will push all your local changes up to the GitHub remote repository.

### Setting up your team
1. Again back over in your favorite web browser go to your github account for the repo you just synced up.  
2. Select the repo settings, which is the gear on the right.
![Github Settings](/images/githubsettings.png)
3. Under settings, click on Collaborators

![Github Collab](/images/SettingsCollaborators.png)

4. On the Collaborators page, you can enter their Github screen names, or their registered email address.

![Collaborators](/images/ghcollabpage.png)


### Pulling the repo to their machines

## The Workflow.
So now we have a team of developers that have copies of the robot code, but what does that get us.  

Well to start, more then one person at a time can write code.  By assigning each coder a function or robotic feature. That coder can create a branch of the master line of code.  Write and test their feature. Then merge their branch back into the master or main line of code.  All of this can be going on while other coders are doing the same process of creating their own branches for a feature they have been been asked to write.  Test that code, and merge it back in with the master line of code.

### But what if? The Dreaded MERGE CONFLICT! - It's not that bad.

What happens if two people edit the same file and the same lines of code?  Well then you have what is called a **Merge Conflict**.  If you try to merge your branch of code in to the master line of code and you have made a change to a line someone else created you will be stopped and asked which line of code to keep.  The original code, or your updated line of code?  
