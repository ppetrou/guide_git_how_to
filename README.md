# Git How to Guide

## Global Configuration

Q. How can I setup global configuration settings?\
A. git config --global GIT_SETTING "GIT_VALUE"\
\
e.g.\
git config --global user.name username\
git config --global user.email usename@email.com

Q. How can I setup local repo configuration settings?\
A. git config GIT_SETTING "GIT_VALUE"\

You need to be in git repo folder for this otherwise you will get a \
fatal: not in a git directory

e.g.\
git config user.name username\
git config user.email usename@email.com


Q. How can I list configuration values\
A. git config -l


Q. Where are the config values stored in a Git Repo?\
A. .git/config

Q. Where are the global config values stored?\
A. ~/.gitconfig

Q. How can i unset a configuration setting?\
A. git config --unset --global GIT_SETTING\
\
e.g.\
git config --unset --global user.name\
git config --unset user.name

Q. How can I set a command alias?\
A. git config --global alias.COMMAND_ALIAS 'GIT_COMMAND'\
\
e.g.\
git config --global alias.ls 'ls-files'


## Remote SSH Access

Q. How can I specify the SSH key to use to authenticate in the Git Server?/
A. You need to following setup in the ~/.ssh/config. Make sure to set the correct private key path and remote user.\
The corresponding public key needs to be set in the Git Server (remote user) in the ~/.ssh/authorized_keys or in https://github.com/settings/keys for GitHub.

```
host github.com
 HostName github.com
 IdentityFile /home/user/.ssh/id_github
 User git

host 192.168.1.100
 HostName 192.168.1.100
 IdentityFile /home/user/.ssh/id_rsa_git
 User git
```


## Repos



## Branches


## Tags


## Remotes


## Commits 

## Merges / Patches


## Stashes


## Hooks







