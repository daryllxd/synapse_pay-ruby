# SynapsePay Ruby Bindings ![Travis CI Status](https://travis-ci.org/synapse_pay/synapse_pay-ruby.svg?branch=master) [![Code Climate](https://codeclimate.com/github/synapse_pay/synapse_pay-ruby/badges/gpa.svg)](https://codeclimate.com/github/synapse_pay/synapse_pay-ruby)


## Installation

You don't need this source code unless you want to modify the gem. If
you just want to use the SynapsePay Ruby bindings, you should run:

```bash
gem install synapse_pay
```

If you want to build & install the gem from source:

```bash
gem build synapse_pay.gemspec
gem install synapse_pay-0.0.1.gem
```





## Requirements

* Ruby 1.8.7 or above. (Ruby 1.8.6 may work if you load
  ActiveSupport.) For Ruby versions before 1.9.2, you'll need to add this to your Gemfile:

```ruby
if Gem::Version.new(RUBY_VERSION) < Gem::Version.new('1.9.2')
  gem 'rest-client', '~> 1.6.8'
end
```

* rest-client, json


## Bundler

If you are installing via bundler, you should be sure to use the https
rubygems source in your Gemfile, as any gems fetched over http could potentially be compromised.

```ruby
source 'https://rubygems.org'

gem 'rails'
gem 'synapse_pay'
```


## Development

Test cases can be run with: `bundle exec rake test`
