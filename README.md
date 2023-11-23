# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


## Install Device in Rails

Add Gem In Gemfile

```bash
  gem "devise" 
```

Run the Command in terminal

```bash
  bundle install 
```
This command will install the Devise gem in your project

```bash
 bundle exec rails g devise:install
```

## 🚀 Display will also be printed in the terminal.

```bash
 Output
===============================================================================

Depending on your application's configuration some manual setup may be required:

  1. Ensure you have defined default url options in your environments files. Here
     is an example of default_url_options appropriate for a development environment
     in config/environments/development.rb:

       config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

     In production, :host should be set to the actual host of your application.

     * Required for all applications. *

  2. Ensure you have defined root_url to *something* in your config/routes.rb.
     For example:

       root to: "home#index"

     * Not required for API-only Applications *

  3. Ensure you have flash messages in app/views/layouts/application.html.erb.
     For example:

       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p>

     * Not required for API-only Applications *

  4. You can copy Devise views (for customization) to your app by running:

       rails g devise:views

     * Not required *

===============================================================================
```

## Run This Command create View Page

```bash
rails g devise:views
```


## Creating the User Model with Devise

```bash
  bundle exec rails g devise user 
```
The following output will print to the screen:
```bash
Output
invoke  active_record
create    db/migrate/20220908152949_devise_create_users.rb
create    app/models/user.rb
invoke    test_unit
create      test/models/user_test.rb
create      test/fixtures/users.yml
insert    app/models/user.rb
route  devise_for :users
```

## Run This command in Terminal

```bash
bundle exec rails db:migrate
```