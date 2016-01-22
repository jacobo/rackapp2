source "https://rubygems.org"

gem "rails", "~> 4.1.9"

gem "pg"

gem "newrelic_rpm"

gem "jquery-rails"

# Use unicorn as the app server
gem "unicorn", ">= 4.8.0pre1"

gem "haml", require: false
gem "haml-rails", require: false
gem "redis"

gem 'chargify2'

gem "zuora", :git => "git@github.com:engineyard/zuora.git", :require => false
# gem "zuora", :path => "../zuora", :require => false

gem "savon", "0.9.9" #Newer versions have incompatible API!
gem "wasabi", "2.1.1" #Newer versions break stuff! (a dep of savon)

gem "httpclient", "~> 2.4.0" #without which: httpi (used by savon), will use net/http

# gem "johnny_cash_api", :path => "johnny_cash_api", require: false
# gem "tresfiestas_api", :path => "../tresfiestas/tresfiestas_api"
gem "tresfiestas_api", ">= 0.0.1"

# Use SCSS for stylesheets
gem "sass-rails"
#, "~> 4.0.3" # fix for sass import failures https://github.com/rails/sass-rails/issues/191

# Use Uglifier as compressor for JavaScript assets
gem "uglifier"#, ">= 1.3.0"

# Use CoffeeScript for .js.coffee assets and views
gem "coffee-rails"#, "~> 4.0.0"

gem "compass-rails"

#TODO: do we want to do this? or handle Zuora::Fault objects before they can make it to broken sinatra code that calls .code and expects an integer
gem "sinatra", :git => "git://github.com/sinatra/sinatra.git", :require => false

gem "fog"
gem "unf"
gem "resque_stuck_queue"
gem "ey_bot", :require => "ey/irc"

gem "resque", :git => "https://github.com/engineyard/resque.git"
gem "async"

gem "state_machine", :git => "https://github.com/engineyard/state_machine.git"

gem "rollbar"
gem "daemons"
gem "multi_headed_greek_monster"

gem "awesome_print"


group :test, :development do
  gem "pry-nav"
  gem "cubbyhole", :require => false
  gem "rspec-rails", ">= 2.0.1", :group => [:development, :test]
  gem "capybara", :require => false
  gem "uuid"
  gem "guard"
  gem "guard-shell"
  gem "launchy"
  gem "timecop"
  gem "simplecov-s3"
  gem "minitest" #not really using it by rails complains without it (maybe future versions of rails won't)
end
