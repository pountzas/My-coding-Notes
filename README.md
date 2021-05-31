# **_My-coding-Notes_**

## GEMS

### **_Rspec_**
- Flexible authentication solution for Rails with Warden

#### Instalation
- creating app without default tests
``rails new your_app_name -t`` 

- need to add devise for genereting tests
``bundle add devise``<br>
``rails g devise:install``<br>
``rails g devise User``<br>

- Next we'll create our posts scaffold.
``rails g scaffold posts title:string body:text user:references views:integer``<br>


 ``rails generate rspec:model User``
#### ```Remove rspec```

- Remove spec directory
- Remove all rspec related gems (capybara, faker, etc.) from the Gemfile
- Run `bundle clean --force` command to remove all unused gems and then run 'bundle install' again
- Now ``bundle list`` should show you all the gems except rspec related

### `Devise`
``bundle add devise``<br>
``rails g devise:install``<br>
``rails g devise User``<br>

### ``fontawesome``
- Run ``yarn add @fortawesome/fontawesome-free``

- Go to javascript/packs/application.js and paste: ``import "@fortawesome/fontawesome-free/css/all"`` 

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

## **_Heroku_**

### Instalation


### push to heroku

``git push heroku main`` or whatever branch
``heroku rename name`` change app name on heroku side