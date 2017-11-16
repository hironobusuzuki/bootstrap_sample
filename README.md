```
$ rbenv local 2.4.1
$ rbenv exec bundle init
$ vi Gemfile
gem "rails"
$ rbenv exec bundle install --path vendor/bundle
$ mv Gemfile Gemfile.bk
$ mv Gemfile.lock Gemfile.lock.bk
$ rbenv exec bundle exec rails new --skip-bundle bootstrap_sample
$ cd bootstrap_sample
$ rbenv exec bundle install --path vendor/bundle
$ rbenv exec bundle exec rails g scaffold book name:string author:string
$ rbenv exec bundle exec rails db:create
$ rbenv exec bundle exec rails db:migrate
$ rbenv exec bundle exec rails s
http://localhost:3000/books
$ vi Gemfile
gem 'jquery-rails'
gem 'jquery-ui-rails'
gem 'bootstrap'
$ rbenv exec bundle install --path vendor/bundle
$ touch app/assets/stylesheets/application.scss
$ rm app/assets/stylesheets/application.css
$ vi app/assets/stylesheets/application.scss
@import "bootstrap";
$ vi app/assets/javascripts/application.js
//= require jquery3
//= require popper
//= require bootstrap-sprockets
$ vi app/views/books/index.html.erb
table class="table table-striped"
$ git config --local user.email hirosuzu001@gmail.com
$ git config --local user.name hironobusuzuki
$ git add *
$ git commit -m 'first commit'
$ git push origin master
```
