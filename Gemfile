# frozen_string_literal: true

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?('/')
  "https://github.com/#{repo_name}.git"
end

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 7.2'
# Ruby 3.4 removed these from default gems; activesupport still requires them
gem 'mutex_m'
gem 'bigdecimal'
# json 3.x dropped the quirks_mode: kwarg that activesupport 7.2's JSON coder still passes
gem 'json', '< 3'
# Use postgresql as the database for Active Record
gem 'pg', '>= 0.18', '< 2.0'
# Use Puma as the app server
gem 'puma', '~> 6.4'
# Use SCSS for stylesheets (Dart Sass via Sprockets; libsass/sassc-rails is EOL)
gem 'dartsass-sprockets'
# Use Terser as compressor for JavaScript assets (uglifier can't handle ES6)
gem 'terser'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'

gem 'activeadmin'
gem 'devise'

gem 'auto_strip_attributes'
gem 'bootstrap', '~> 4.3'
gem 'jquery-rails'
gem 'rack-canonical-host'
gem 'recaptcha', require: 'recaptcha/rails'
gem 'scenic'

group :development, :test do
  gem 'rubocop'
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: %i[mri mingw x64_mingw]
  # Adds support for Capybara system testing and selenium driver
  gem 'capybara', '~> 2.13'
  gem 'selenium-webdriver'
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'listen', '~> 3.3'
  gem 'web-console', '>= 3.3.0'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end
