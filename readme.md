# FRC Robot Example using git & github

Trying to get the process down on how to setup a new robot project, put it under git control, setup a remote repo and push local changes up to github.

## Dependency 
* Download and install the *WPI/VS Code extensions*, along with the *WPILIB*. Here are the [FIRST Screensteps](http://wpilib.screenstepslive.com/s/currentCS/m/getting_started) for the setting up the 2019 Control System. There is a link to the offline installer. It's 1 gig in size, so make sure you've got the bandwidth or data limits.
* git - You will need to have a local version of git installed so you can work with your coding team on github.
    * Windows users will need to download and install a version of git. [Click Here](https://git-scm.com/downloads/win) to download Git for Windows.  
    * Most Linux might have it installed already.  Open a terminal and enter git.  If you get an error, you most likely need to install it. [Great Instructions for doing that are just a click away.](https://git-scm.com/download/linux)
    * Mac users can also use this [link to download](https://git-scm.com/download/mac) for Mac OSx
    * Make sure to check out the [git docs online](https://git-scm.com/docs)
* VS Code does have support for git built in, but under the market place there are maybe wonderful extensions. GitLens being one I really like. Also in the VS Code market place "Github Pull Requests".  Allowing you to submit a remote Pull Request (also know as a PR) right from the comfort of your editor.

## Process Overview
1. In VS Code, bring up the WPILIB command pallet. 
2. Select "Create new project"
3. Enter all the basic project information. Make sure that the "Create new folder" checkbox is selected.  This will generate all the basic project files, java templates, gradle settings, etc...
4. 