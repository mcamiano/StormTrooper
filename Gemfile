source 'https://rubygems.org' 

# Use e.g. $ bundle install --without production [development] [test]
# to exclude one or more groups
#
# See http://bundler.io/v1.6/groups.html
#
# The :default group includes any gems not in a named group
#
group :development do
end

group :test do
end

group :production do
end

group :development, :test, :production do
  # 
  # https://github.com/capistrano/bundler
  #
  gem 'capistrano', '~> 3.1.0'
  gem 'capistrano-composer'
  
  # gem 'capistrano-bundler', '~> 1.1.2'
end

# gem 'cucumber', :group => [:cucumber, :test] 

