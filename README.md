# My-coding-Notes

## GEMS

### ```Remove rspec```

1) Remove spec directory
2) Remove all rspec related gems (capybara, faker, etc.) from the Gemfile
3) Run `bundle clean --force` command to remove all unused gems and then run 'bundle install' again
4) Now ``bundle list`` should show you all the gems except rspec related
