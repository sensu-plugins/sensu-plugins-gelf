## Sensu-Plugins-gelf

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-gelf.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-gelf)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-gelf.svg)](http://badge.fury.io/rb/sensu-plugins-gelf)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-gelf/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-gelf)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-gelf/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-gelf)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-gelf.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-gelf)
[ ![Codeship Status for sensu-plugins/sensu-plugins-gelf](https://codeship.com/projects/536cdd50-ea30-0132-e9f0-32dfa18a9fce/status?branch=master)](https://codeship.com/projects/83068)

## Functionality

## Files
 * bin/handler-gelf

## Usage

```
{
  "gelf": {
    "server": "graylog.dom.tld",
    "port": "12201"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-gelf -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-gelf`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-gelf' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-gelf' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
