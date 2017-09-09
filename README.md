# Ruby on Rails Tutorial

## "hello, world!"

This is the first application for the
[*Ruby on Rails Tutorial*](http://railstutorial.jp/)
by [Michael Hartl](http://www.michaelhartl.com/). Hello, world!



# Hroku upload

$ heroku login
Email:
Password:

下記追加
group :production do
  gem 'rails_12factor'
end

config/environments/production.rb
config.assets.comppile = true 変更

$ heroku create
Creating app... done, ⬢ still-beyond-43032
https://still-beyond-43032.herokuapp.com/ | https://git.heroku.com/still-beyond-43032.git
アプリ名：still-beyond-43032

$ heroku addons:add cleardb

$ heroku config | grep CLEARDB_DATABASE_URL

$ heroku addons:detach DATABASE -a still-beyond-43032

$ heroku config:add DATABASE_URL='mysql2://xxxxxxxxx'

$ heroku config

$ git push heroku master

$ heroku run rake db:migrate
