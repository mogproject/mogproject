Setup GitHub 
====

### Prerequisite

- Python2

```
$ brew install reattach-to-user-namespace
$ brew python
```

- Git

```
$ ln -s $DROPBOX_DIR/config/_gitconfig ~/.gitconfig
```

### Create and register SSH key

```
$ ssh-keygen -t rsa -b 4096 -C "mogproj@gmail.com" -f ~/.ssh/mogproject.github
Enter passphrase (empty for no passphrase): [***secret***]
Enter same passphrase again: [***secret***]
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/mogproject.github
$ pbcopy < ~/.ssh/id_rsa.pub
```

- Register: https://github.com/settings/ssh

### Configure SSH

```
host github.com
 HostName github.com
 IdentityFile ~/.ssh/mogproject.github
 User git
```

### Test

```
$ ssh -T git@github.com
```

### Clone repositories

```
$ sudo mkdir -p /proj && sudo chown $USERNAME:staff /proj
$ cd proj
$ mkdir mogproject
$ git clone git@github.com:mogproject/mogproject.git
```
