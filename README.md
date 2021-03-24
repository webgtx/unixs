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
