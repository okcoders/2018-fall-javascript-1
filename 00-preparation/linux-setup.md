Linux Instructions
====

## Install software

Most Linux users are already familiar with the install processes of their 
systems.  However, Chrome will need to be downloaded separately due to 
licensing issues on most platforms. Download the appropariate package for your
Linux system here:

[Google Chrome](https://www.google.com/intl/en-US/chrome/browser/)

Google Chrome has excellent developer tools that we will utilize when we get
into scraping websites.  Chromium is also available and is basically the 
development version of Chrome.

Additionally you will need a text editor.  If you want a built in one you can
try __kate__ or if you do not already have a preferred editor, then check out 

[Visual Studio Code](https://code.visualstudio.com/)

Once you've installed VSCode, make sure to also install the command line tool. 

1. While VSCode is open, open the command palette by pressing `ctrl + shift + p`
	- the command palette contains commands that your text editor can perform (eg. creating a new file, copying a file, etc.)
2. Type `install command`, and select the first option that reads

```
Shell Command: Install 'code' command in PATH
```

3. Close VSCode and any terminal windows you might have open, and reopen the terminal.
4. Type `code` into the terminal and VSCode should launch.

This is what I will be using in the class, with a few quality of life extensions installed. 

Finally, you will need to install Node.js, git, and mongodb.  They can all be
install with your systems standard software installer via:

### Redhat, Fedora, CentOS

As root run the following command:

```bash
dnf install git nodejs 
```

### Debian, Ubuntu

As root run the following command:

```bash
sudo apt-get -y install git nodejs 
```

## Configure Git

Set your global git user name and email. At the terminal, type the following two commands. **Note: The email address should be the same as your github account.** Press enter after each one:

	git config --global user.name "Your Name"
	git config --global user.email your@email.address

## Set up your SSH keys

SSH Keys are used to establish a secure connection to GitHub and Heroku.

Follow the instructions at GitHub to create and register new SSH keys: [Generating SSH Keys for GitHub](https://help.github.com/articles/generating-ssh-keys).

Note: When you're entering a password during this process it **will not** show up in the terminal. This is for security reasons.

If you get an error when trying to add your keys to the ssh-agent, type the following command at the terminal prompt and press return:

	eval `ssh-agent -s`

Nice work! You just set up your development environment and are already using the command line! This is serious stuff!
