# 🧙‍♀️ command-line-magic 

### ✨ Caching git password

#### HTTPS clone

##### Linux 
Set git to use the credential memory cache
```
git config --global credential.helper cache
```

To change the default password cache timeout
```
git config --global credential.helper 'cache --timeout=10800'
```

##### Mac OS
1. Check if `osxkeychain helper` is installed
```
git credential-osxkeychain
```
2. Set git to use the `osxkeychain helper`
```
git config --global credential.helper osxkeychain
```

### ✨ Changing use credentials in a particular repository
Clear local git credentials
```
git config --local credential.helper ""
```
the proceed with the git operations you want to perform. You will be prompted to enter credentials again.

### ✨ Revert unpushed Git commits
Delete the most recent commit, keeping the work you've done:
```
git reset --soft HEAD~1
```

Delete the most recent commit, destroying the work you've done:
```
git reset --hard HEAD~1
```

### ✨ Find remote URL of a Git repository
```
git config --get remote.origin.url
```
