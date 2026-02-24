
Day 2: Users, Permissions & Important Directories

Objective of day 2 :
Understanding linux file permissions, user roles (Root vs. Normal User), and explore the system's directory hierarchy.

Tasks that I performed today :

1. Folder and file creation
* Created `Day02Practice` folder in the home directory.
* Created `test1.txt` and `test2.txt` inside.

2. Permission experiment (The "Permission Denied" Test)
* The Discovery: While logged in as `root`, I noticed that removing write permissions (`chmod u-w`) did not stop me from editing the file.
* The Solution: I switched to my normal user (`stark`).
* The Result: After running `chmod u-w test1.txt`, I attempted to use `echo "Hello" > test1.txt`.
* Observation: The terminal correctly returned `zsh: permission denied: test1.txt`.
* Restoration: I ran `chmod u+w test1.txt` and confirmed I could write to the file again.

3. Directory exploration 
I explored the following key linux directories:
* `/home`: Contains the personal folder for user `stark`.
* `/etc`: Found system configuration files (the "Control Panel").
* `/var`: Viewed variable data and logs.
* `/tmp`: Found temporary files used by the system.
* `/bin`: Observed essential command binaries like `ls` and `cp`.


What did I learn today: 

1. Normal user vs. root: A normal user is restricted by permissions to protect the system. The `root` user is the superuser and can bypass these restrictions.
2. Sudo: Used when a normal user needs to perform a command that requires root-level authority.
3. Importance of permissions: They are the first line of defense in Linux, ensuring users don't accidentally or intentionally delete system-critical files in directories like `/etc` or `/bin`.
