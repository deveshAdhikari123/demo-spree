# README

* Ruby version
  2.6.3

* Installation

   bundle install

   *Note: if you run into Bundler could not find compatible versions for gem "sprockets": error message, please run
   bundle update


Use the install generators to set up Spree:
  bundle exec rails g spree:install --user_class=Spree::User
  bundle exec rails g spree:auth:install
  bundle exec rails g spree_gateway:install

# Installation options
  By default, the installation generator (rails g spree:install) will run migrations as well as adding seed and sample data and will copy storefront data for easy customization (if spree_frontend available). This can be disabled using
  rails g spree:install --migrate=false --sample=false --seed=false --copy_storefront=false

You can always perform any of these steps later by using these commands.

bundle exec rake railties:install:migrations
bundle exec rails db:migrate
bundle exec rails db:seed
bundle exec rake spree_sample:load
bundle exec rails g spree:frontend:copy_storefront

# Browse Storefront
Go to http://localhost:3000

# Browse Admin Panel
Go to http://localhost:3000/admin

# Admin panel credentials for your own Heroku demo:

 login: spree@example.com
 password: spree123



* ...
