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
