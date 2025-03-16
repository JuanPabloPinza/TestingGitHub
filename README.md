# Testing GitHub
Testing GitHub options.
Editing this with github.dev

## Cloning
There are 3 ways: HTTPS, SSH, GitHub CLI.
### HTTPS
```sh
git clone https://github.com/JuanPabloPinza/TestingGitHub
```
> For this you could access with your credentials or generate a Personal Access Token (PAT).
https://github.com/settings/token
### SSH
You can also access your repo via SSH, but you have to get a sshkey.
```sh
ssh-keygen -t rsa
```
One you create your SSH Key you can access your repo, you need to add the Generated SSH Key into your GitHub account.
> You have to know that you also have to add the SSH key in your computer first.

```sh
sshe-keygen -t rsa
```
> You also have to activate the SSH option in your PC

### CLI
You can also clone using the CLI, and you have to install it first

#### There is a Git hidden folder called '.git'
So if you want to create a git repo in a new folder the first thing you gotta do is create the folder and initialize.

## Set the global editor
Git needs credentials to identify the person who is changing files in the repo.
In his case the default is:
```sh
git config --global core.editor emacs
```
## Set the gitconfig files
Stores your global git configuration.
To show your configurations:
```sh
git config --list
```
E.g. to set up your name and email for the first time:
```sh
git config --global user.name "Juan Pablo Pinza"
git config --global user.email "test@gmail.com"
```


## Add
This command is used to stage files.
```sh
git add testing.md
```
## Reset
Allows you to remove staged changes to be unstaged.
```sh
git reset testing.md
```

## Branches

To check the branches:
```sh
git branch
```
To create a new/move to a branch
```sh
git checkout branch-name
```
