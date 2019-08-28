# command-line-magic

### 1. Caching Git Password

#### HTTPS clone

1. Check if `osxkeychain helper` is installed
```
git credential-osxkeychain
```
2. Set git to use the `osxkeychain helper`
```
git config --global credential.helper osxkeychain
```
