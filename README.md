# Git Steps Cheatsheet

## Start SSH-AGENT
```
eval `ssh-agent.exe`
```

## Checking for SSH Key Connection to Github
```
ssh -T git@github.com
```

## Generating new SSH Key and Adding to GitHub
Check this link: https://www.toolsqa.com/git/ssh-authentication-in-git/

## Cloning a repository:
```
git clone git@github.com:TheEverlastingBish/horny-rhino.git
```

## Working with Git Bash

#### Navigate to the newly created local copy of remote repository
```
cd horny-rhino
```

#### Initialise the directory as a git repo
```
git init
```

#### Check status to make sure it's ready for editing
```
git status
```

#### Edit files or folders as required


#### Add edited files to commit
```
git add 'filename.ext'
git add .
```

#### To commit
```
git commit -m "This is the commit message"
```

#### To amend last commit
```
git commit --amend -m "This is the amended commit message"
```

#### To check log
```
git log --oneline
git log --pretty=oneline
```
## Pushing to Remote

#### Standard push to remote
```
git push origin master
```


#### To force a new push over the last commit
```
git push --force origin master
```


## Tags (for versioning)
#### See existing tags
```
git tag
git tag -l
```

#### Adding a tag / milestone
`git` `tag` `[version_or_tag_name_you_want]` `[commit id]` `[-m]` `[message]`
```
git tag v1.0.0 0af465d2f72edccc2acd48d176e7918bf73181fe -m "First complete version"
```

#### Pushing tag to repo
```
git push origin v1.0
```

#### Pushing multiple un-pushed tags all at once
```
git push origin --tags
```

#### Deleting a local tag
```
git tag -d v1.0
```

#### Deleting a remote tag
```
git push --delete origin v1.0
```

