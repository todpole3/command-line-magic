# command-line-magic

### 🔨 Caching Git Password

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
