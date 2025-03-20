# **Experiment - 7 & 8**

_Create the `/home/consultants` directory. Add write permission to the consultants group. Use the symbolic method for setting the appropriate permissions. Forbid others from accessing files in the `/home/consultants` directory. Use the octal method for setting the appropriate permissions. Change the default umask for the operator1 user. The new umask prohibits all access for users that are not in their group. Confirm that the umask is changed._

#

### **Approach**

Use `mkdir` to create a directory. Modify permissions using the symbolic method (`chmod g+w`) and the octal method (`chmod 770`). Update the `umask` setting for `operator1`.

### **Syntax**

**`sudo mkdir /home/dir1`**  
Creates a directory named `/home/dir1` with superuser (root) privileges.

**`sudo chmod g+w /home/dir1`**  
Grants write permissions to the group for the `/home/dir1` directory.

**`sudo chmod 770 /home/dir1`**  
Sets the permissions for the `/home/dir1` directory to `rwxrwx---`, allowing the owner and group to read, write, and execute, while others have no permissions.

**`sudo su - user1`**  
Switches to the `user1` user with root privileges, starting a login shell.

**`echo "umask 007" >> ~/.bashrc`**  
Appends `umask 007` to the `~/.bashrc` file, which sets the default permissions for newly created files and directories to `770`.

**`source ~/.bashrc`**  
Reloads the `~/.bashrc` file to apply the changes.

**`umask`**  
Displays the current umask value.

### **Example**

```
sudo mkdir /home/consultants

```

```
sudo chmod g+w /home/consultants

```

```
sudo chmod 770 /home/consultants

```

```
ls -ld /home/consultants

```

```
sudo su - operator1

```

```
echo "umask 007" >> ~/.bashrc

```

```
source ~/.bashrc

```

```
umask

```

Confirm `umask`

```
touch testfile
mkdir testdir
ls -l
```

#
![4 1](https://github.com/user-attachments/assets/16da8142-1c61-4432-9dc9-2f211aa58bac)
![4 2](https://github.com/user-attachments/assets/5c5e2351-57cd-4953-981f-1596abb1553a)
![4 3](https://github.com/user-attachments/assets/e80dbd49-fc73-48e3-b784-37649f513981)
![4 4](https://github.com/user-attachments/assets/0b76aadc-8ad5-4e59-9f72-85c5eec3483f)
