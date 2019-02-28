#### Existing repo to new repo
Clone old repo
```bash
$ git clone old_repo.git
```
Update git remote origin URL to new repo url
```bash
$ vim .git/config
```
Check if remote origin is right
```bash
$ git remote -v
```
If remote origin is set, push to master
```bash
$ git push origin master
```


#### Levels of git config
Project Level
```bash
$ git config user.name "Krista Mae Rectra" 
```
Global Level
```bash
$ git config --global user.name "Krista Mae Rectra"
```
System Level
```bash
$ git config --system user.name "Krista Mae Rectra" 
```