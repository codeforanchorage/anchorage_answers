source 'https://rubygems.org'

#gem 'bundler', '~> 1.3.0.pre.5' # Bundler version to match what is used on Heroku.

## Essentials
ruby '1.9.3' # Ruby!
gem 'rails', '3.2.16' # Rails!
gem 'pg', '~> 0.17.0' # PostgreSQL, the database server
gem 'thin', '~> 1.5.0' # Web server

gem 'newrelic_rpm', :group => [:production, :staging, :development] # Rails analytics - see the Heroku addon
gem 'progressbar', '~> 0.12.0' # Display progress bars in terminal output
gem 'facets', :require => false # Some extra methods for ruby
gem 'jquery-ui-rails', '~> 3.0.1' # Package jQuery for the Rails 3.1+ asset pipeline
gem 'rollbar', '~>0.10.11' # SaaS to track exceptions

## SEO
gem 'meta-tags', :require => 'meta_tags' # Search Engine Optimization (SEO) plugin for Ruby on Rails applications.

## Performance and optimization
gem 'delayed_job_active_record', '~> 0.3.3' # Lets you queue tasks as background jobs
gem 'dalli', '~> 2.6.0' # memcache gem for Rails.cache
gem 'memcachier', '~> 0.0.2'
gem 'kgio', '~> 2.7.4' # gives 20~30% performance boost to Dalli

## Admin
gem 'activeadmin', '~> 0.6.0' # Back-end Content Management System
gem 'devise', '~> 2.2.1' # User authentication
gem 'cancan', '~> 1.6.8' # User permissions

## Search and NLP
gem 'tanker', '~> 1.1.6' # library for interacting with Searchify
#gem 'hunspell-ffi' # Spellchecking library
gem 'text', '~> 1.2.1' # NLP algorithms
gem 'httparty', '~> 0.10.0' # For accessing APIs directly
gem 'json', '~> 1.8.1' # Convert between JSON and Ruby objects

## Content and presentation
gem 'kramdown', '~> 0.14.1' # Better markdown parser with support for markdown-extra
gem 'friendly_id', '~> 4.0.9' # Create permalinks / descriptive URLs / slugs
gem 'paperclip', '~> 3.0' # Easy file attachment library for ActiveRecord
gem 'aws-sdk', '~> 1.3.4' # Upload files to Amazon S3

## Gems used only for assets and not required
## in production environments by default.
group :assets do
  gem 'sass-rails', '~> 3.2.5' # Rails support for Sass, a CSS extension language
  gem "meta_search", '>= 1.1.0.pre' # Active_admin search for form_for
  gem 'uglifier', '>= 1.0.3' # Squash down Javascript for speed
  gem 'coffee-rails', '~> 3.2.1'
  gem 'therubyracer', '~> 0.12.0' # Embeds the V8 Javascript interpreter into Ruby
end

## Testing
group :test, :development do
  gem 'rspec-rails', '>= 2.0' # Testing framework
  gem 'shoulda', '~> 3.5.0' # Extra RSpec matchers for Active Record Associations
  gem 'factory_girl_rails', '~> 4.0' # Create factories to test against
  gem 'capybara', '~> 2.1'
  gem 'guard', '~> 1.8.0'
  gem 'guard-rspec', '~> 3.0.0'
  gem 'terminal-notifier-guard', '~> 1.5.3'
  gem 'sextant', '~> 0.2.3' # visit /rails/routes in the browser for nicer 'rake routes'
  gem 'memcached', '~> 1.5.0' # Local memcache
  gem 'seed_dump', '~> 0.6.0' # Adds rake db:seed:dump to generate db/seeds.rb
end

group :production do
  gem 'rails_12factor', '~> 0.0.2'
end

group :test do
  gem "sqlite3", '~> 1.3.6' # Use SQLite instead of PostgreSQL for tests
end
