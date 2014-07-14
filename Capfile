# Capistrano composer package
# https://github.com/capistrano/composer
# Allows:
# composer:install
# composer:install_executable
# composer:dump_autoload
# composer:self_update
# composer:run
#
# e.g. cap production composer:run['status','--profile']
#
require 'capistrano/composer'

# set :composer_install_flags, '--no-dev --no-interaction --quiet --optimize-autoloader'
# set :composer_roles, :all
# set :composer_dump_autoload_flags, '--optimize'
# set :composer_download_url, "https://getcomposer.org/installer"
# set :composer_version, '1.0.0-alpha8' #(default: not set)
#
#
# Install composer as part of the deployment into shared path
SSHKit.config.command_map[:composer] = "php #{shared_path.join("composer.phar")}"

namespace :deploy do
  before :starting, 'composer:install_executable'
end


# http://jeremykendall.net/2013/11/24/php-and-capistrano-3-notes-to-self/
# http://capistranorb.com/
