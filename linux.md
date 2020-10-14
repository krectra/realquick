### Copy
#### Copy folder contents to another folder
```bash
$ cp -a /source/. /dest/
```

### Filesystem
#### Traverse and display size
```
$ du -shx /* | sort -rh
```

### User
#### Add user
```bash
$ adduser username
```
#### Change user password
```bash
$ sudo passwd username
```
#### Add user to the `sudo` group
```bash
$ usermod -aG sudo username
```
##### To test for sudo
```bash
$ su - username
```
```bash
$ sudo ls -la /root
```

#### Delete user
```bash
$ sudo userdel username
```
#### Delete user home directory
```bash
$ sudo rm -r /home/username
```




Reference:
- https://www.cyberciti.biz/faq/create-a-user-account-on-ubuntu-linux/
