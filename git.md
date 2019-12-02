#### Tag
Delete
```
$ git push --delete origin <tag_name>
```
Remove local git tags that are no longer on the remote repository
```
$ git tag -l | xargs git tag -d
$ git fetch --tags
```

#### Existing project to new repo
```bash
$ git init
```
Add initial files
```bash
$ git add <file_to_add>
```
Commit
```bash
$ git commit -m "First commit"
```
Add remote repo URL
```bash
$ git remote add origin <remote_repository_url>
```
Verify
```bash
$ git remote -v
```
Push
```bash
$ git push origin master
```

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

#### Changing a remote's URL
To change
```bash
$ git remote set-url origin https://github.com/<user_name>/<repository>.git
```
To verify
```bash
$ git remote -v
```
Alternative:
Edit via `.git/config`
```bash
$ vim .git/config
```
Look for the `[remote "origin"]`, and edit its URL
```
[remote "origin"]
url = https://github.com/<user_name>/<repository>.git
```


#### Renaming local git branch
```bash
$ git branch -m <old_branch_name> <new_branch_name>
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
