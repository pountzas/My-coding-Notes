# **_My-coding-Notes_**

## **_git/github_**
Magic link
https://www.freecodecamp.org/news/git-cheat-sheet/

### deleete a branch localy
```git branch -D friendshipsV2```

### Unstaging 1 file from added files to stage

```git restore .\spec\models\frienship_spec.rb --staged```

### Undo changes since last commit:

```git clean -fd```
<br>
```git reset --hard```

### Delete last commit from github

- Load previus commit
- Push by force to roleback and delete commits fro github

```git reset HEAD^ --hard```<br>
```git push -f```

### Uncheck last commit

```git reset --soft HEAD~1```

### Use subtree push to send it to the gh-pages branch on GitHub.

```git subtree push --prefix dist origin gh-pages```<br>
Boom. If your folder isn’t called dist, then you’ll need to change that in each of the commands above.

## **_Heroku_**

### Instalation


### push to heroku
```git heroku create```
```git push heroku main```<br>
or whatever branch<br>
```heroku rename name```<br> change app name on heroku side

https://devcenter.heroku.com/articles/getting-started-with-rails5

#### to change the stack 
```heroku stack:set heroku-18 --app ror-social-friends```

#### when deploy and “We're sorry, but something went wrong.”
```heroku rake db:migrate --app ror-social-friends```<br>
```heroku restart --app ror-social-friends```
