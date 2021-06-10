# **_My-coding-Notes_**

## RoR 

### **_Create_**
``rails new appName``<br>
``rails new .//``<br> 

### **_server_**
``rails s``<br>
``rails server -e production -p 4000``<br> change server  port

### drop db inside rails console only that table
``Friendship.delete_all``

## GEMS

### **_Rspec_**
- Flexible authentication solution for Rails with Warden

#### Instalation
- creating app without default tests<br>
``rails new your_app_name -t`` 

- need to add devise for genereting tests<br>
``bundle add devise``<br>
``rails g devise:install``<br>
``rails g devise User``

- Next we'll create our posts scaffold.<br>
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

### ``has_friendship``<br>
- gemfile <br>
``gem 'has_friendship'``<br>
``rails has_friendship_engine:install:migrations``<br>
``rake db:migrate``

### ``simple forms``
- gemfile <br>
``gem 'simple_form'``<br>

#### instalation
- Run the following command to install it:<br>
``bundle install``

- Run the generator:

``rails generate simple_form:install`` or<br>
``rails generate simple_form:install --bootstrap``- 

### ``fontawesome``
- Run ``yarn add @fortawesome/fontawesome-free``

- Go to javascript/packs/application.js and paste: ``import "@fortawesome/fontawesome-free/css/all"`` 

## **_git/github_**
Magic link
https://www.freecodecamp.org/news/git-cheat-sheet/

### deleete a branch localy
``git branch -D friendshipsV2``

### Unstaging 1 file from added files to stage

``git restore .\spec\models\frienship_spec.rb --staged``

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

``git push heroku main``<br>
or whatever branch<br>
``heroku rename name``<br> change app name on heroku side

https://devcenter.heroku.com/articles/getting-started-with-rails5
