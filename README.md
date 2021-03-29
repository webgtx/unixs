# Welcome to the CheatSheet for UNIX.

There will be a cheat sheet map, watch and open the topic you need.

1.  GIT.

2.  Security, Access Rights, Users and Groups.

3.  Directory commands.





## 1. What is Git?

So, what is Git in a nutshell?
This is an important section to absorb, because if you understand what 
Git is and the fundamentals of how it works, then using Git effectively 
will probably be much easier for you.
As you learn Git, try to clear your mind of the things you may know 
about other VCSs, such as CVS, Subversion or Perforce — doing so will 
help you avoid subtle confusion when using the tool.
Even though Git’s user interface is fairly similar to these other VCSs, 
Git stores and thinks about information in a very different way, and 
understanding these differences will help you avoid becoming confused 
while using it.

<div>
    <img alt="" src="https://git-scm.com/book/en/v2/images/areas.png">
</div>

## 1.2 GIT commands:

<div>
     <img alt="" src="https://cusy.io/images/git-cheat-sheet-2.png/image">
</div>

## 2.0 Security, Access Rights, Users and Groups:

### Creating user and groups

First of all we need to make user

```bash
sudo useradd -m -s /bin/bash $name_of_user
```

u can use  flag -p to add password for example

```bash
sudo useradd -m -s /bin/bash -p $password $name_of_user
```

### Groups of users

You can create as many groups as you want and give them some rights so they won't be able to read , write, run some files

```bash
sudo gpasswd -a $name_of_user $name_of_group
```

If you want to remove user from group you should use -d flag example:

```bash
sudo gpasswd -d $name_of_user $name_of_group
```

### Deleting user

If you do not need some users any more you can easily delete them using this command:

```bash
sudo userdel $name_of_user
```

### Setting password for user

If you have problems with setting password you can use this command:

```bash
passwd $name_of_user
```
