Windows Instructions
====

You must be running a recent version of Windows, at least Windows Vista or higher. Windows 7 or higher is strongly recommended. Ensure that you have installed the latest Windows updates for you version of windows.

## Install software

Install the following software by downloading it at these urls:

* [Sublime Text](https://www.sublimetext.com/).
* [Visual Studio Code](https://code.visualstudio.com/)

This is the free text editor we will be using in class.

[Google Chrome](https://www.google.com/intl/en-US/chrome/browser/).

We will be doing all web development in Google Chrome because of its excellent developer tools.

[Git Bash](http://msysgit.github.io/)

Windows does come with a built-in command prompt, but we will be using another Terminal emulator with built-in support for git, the version control software that works with GitHub. *Do not use the built-in command prompt*. Use Git Bash.

## Configure Git

Set your global git user name and email. At the terminal, type the following two commands. Press enter after each one:

	git config --global user.name "Your Name"
	git config --global user.email your@email.address

## Install Node and Friends

Install Node.js: [http://nodejs.org/](http://nodejs.org/).

Install Express:  Launch Git Bash from your Start menu and at the terminal, type the following two commands and press return after each one to execute it:

	npm install -g express-generator

## Set up your SSH keys

SSH Keys are used to establish a secure connection to GitHub and Heroku.

Follow the instructions at GitHub to create and register new SSH keys: [Generating SSH Keys for GitHub](https://help.github.com/articles/generating-ssh-keys).

If you get an error when trying to add your keys to the ssh-agent, type the following command at the terminal prompt and press return:

	eval `ssh-agent -s`

