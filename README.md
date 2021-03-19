# test2

## Project setup on windows
### Create remote repo, ssh keys, check git config
```
https://sergeyvasin.net/2017/03/30/git-ssh/
git config --global user.email ""
git config --global user.name ""
```
### Create vuetify project
```
vue create my-app
cd my-app
vue add vuetify
```
### Init local repo and link it to remote
```
git init
git add ./
git commit
git branch -M main
git remote add origin git@github.com:CHERNOMORGAMES/test2.git
git push -u origin main
```

### Comment or remove /dist in .gitignore
```
# /dist
```
### Add publicPath in vue.config.js
```
module.exports = {
	publicPath: '/test2',
  transpileDependencies: [
    'vuetify'
  ]
}
```
### Create deploy.sh file in project root
```
https://cli.vuejs.org/ru/guide/deployment.html#github-pages
```
### Edit and Run deploy.sh
```
deploy.sh
```
### Check GH pages settings on github.com