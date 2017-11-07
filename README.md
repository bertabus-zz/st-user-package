# st-user-package

SublimeText User package, all my settings and configs needed to use sublime text between computers.

# Setup a New PC with these settings

quick setup steps taken from [here.](https://forum.sublimetext.com/t/what-s-the-best-way-to-backup-the-st3-configuration/25494/2)

1) remove the User folder of the fresh install

```sh
# Common Linux Path
rm -rf ~/.config/sublime-text-3/Packages/User/
```

```sh
# Common Mac OS Path
rm -rf ~/GetPathOfThisFolderLater/
```

2) clone your backup (only the User folder)

```sh
# Linux
git clone git@github.com:bertabus/st-user-package ~/.config/sublime-text-3/Packages/User/
```

```sh
# Mac OS
git clone git@github.com:bertabus/st-user-package ~/GetPathOfThisFolderLater/
```

3) install Package Control

instructions at the [package control website.](https://packagecontrol.io/installation)

4) restart Sublime Text

# creating your own with existing settings
If you want to make your own repo with existing settings that you already have
just follow along below. Note that I would copy .gitignore settings prior to doing this.

```sh
# CD /path/to/UserFolder/ 
# See first command for common locations
# Make sure to copy .gitignore first, also adjust ssh below for https as appropriate
git init
git remote add origin  git@github.com:USERNAM/st-user-package
git remote set-url origin git@github.com:USERNAME/st-user-package
git pull origin master
git status
git add *
git commit -m "initial commit of user files"
git push
git push origin master
```
