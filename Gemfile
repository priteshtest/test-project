source "https://rubygems.org"

#git_source(:github) do |repo_name|
#  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
#  "https://github.com/#{repo_name}.git"
#end

# We need a newish Rake since Active Job sets its test tasks' descriptions.
#gem "rake", ">= 11.1"

# This needs to be with require false to ensure correct loading order, as it has to
# be loaded after loading the test library.
#gem "mocha", "~> 0.14", require: false

#gem "rack-cache", "~> 1.2"
gem "jquery-rails"
gem "coffee-rails"
gem "sass-rails"
gem "turbolinks", "~> 5"

# require: false so bcrypt is loaded only when has_secure_password is used.
# This is to avoid Active Model (and by extension the entire framework)
# being dependent on a binary library.
gem "bcrypt", "~> 3.1.11", require: false

# This needs to be with require false to avoid it being automatically loaded by
# sprockets.
gem "uglifier", ">= 1.3.0", require: false
gem "sass", github: "sass/sass", branch: "stable", require: false
gem "rb-inotify", github: "matthewd/rb-inotify", branch: "close-handling", require: false

# Explicitly avoid 1.x that doesn't support Ruby 2.4+
gem "json", ">= 2.0.0"

gem "rubocop", require: false

group :doc do
  gem "sdoc", "1.0.0.beta2"
  gem "redcarpet", "~> 3.2.3", platforms: :ruby
  gem "w3c_validators"
  gem "kindlerb", ">= 1.0.1"
end

# Active Support.
gem "dalli", ">= 2.2.1"
gem "listen", ">= 3.0.5", "< 3.2", require: false
gem "libxml-ruby", platforms: :ruby

# Active Job.
group :job do
  gem "resque", github: "resque/resque", require: false
  gem "resque-scheduler", require: false
  gem "sidekiq", require: false
  gem "sucker_punch", require: false
  gem "delayed_job", require: false, github: "collectiveidea/delayed_job"
  gem "queue_classic", github: "QueueClassic/queue_classic", branch: "master", require: false, platforms: :ruby
  gem "sneakers", require: false
  gem "que", require: false
  gem "backburner", require: false
  #TODO: add qu after it support Rails 5.1
  # gem 'qu-rails', github: "bkeepers/qu", branch: "master", require: false
  gem "qu-redis", require: false
  gem "delayed_job_active_record", require: false, github: "collectiveidea/delayed_job_active_record"
  gem "sequel", require: false
end

# Action Cable
group :cable do
  gem "puma", require: false

  gem "em-hiredis", require: false
  gem "hiredis", require: false
  gem "redis", require: false
end


