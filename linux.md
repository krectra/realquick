### User
#### Add user
```bash
$ adduser username
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


### Copy
#### Copy folder contents to another folder
```bash
$ cp -a /source/. /dest/
```
