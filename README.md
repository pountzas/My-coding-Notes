# **_My-coding-Notes_**

## GEMS

### **_Rspec_**


#### ```Remove rspec```

- Remove spec directory
- Remove all rspec related gems (capybara, faker, etc.) from the Gemfile
- Run `bundle clean --force` command to remove all unused gems and then run 'bundle install' again
- Now ``bundle list`` should show you all the gems except rspec related

### `Devise`

## **_git/github_**
Magic link
https://www.freecodecamp.org/news/git-cheat-sheet/

### Undo changes since last commit:

``git clean -fd
``<br>``
git reset --hard``

### Delete last commit from github

- Load previus commit
- Push by force to roleback and delete commits fro github

``git reset HEAD^ --hard
``<br>``
git push -f``

### Uncheck last commit

``git reset --soft HEAD~1``
