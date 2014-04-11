# Fluent::Plugin::NginxStatus, a plugin for [Fluentd](http://fluentd.org)

## Installation

Add this line to your application's Gemfile:
    gem 'fluent-plugin-nginx-status'

Or install it yourself as:
    $ gem install fluent-plugin-nginx-status

Or use td-agent : (on Ubuntu12.04)
    $ sudo /usr/lib/fluent/ruby/bin/fluent-gem install fluent-plugin-nginx-status

## Configuration

Adding the following source block will enable the nginx status plugin for FluentD

    <source>
        type nginx_status
        tag  nginx.status.localhost
    </source>

You also need to enable the nginx_status page in your nginx configuration, see the following link for more details:

http://wiki.nginx.org/HttpStubStatusModule

## Options
| Key           | Default       | Required  |
|:------------- |:-------------:|:---------:|
| tag           | nginx.status  |    yes    |
| host          | 127.0.0.1     |    no     |
| port          | 80            |    no     |
| path          | /nginx_status |    no     |
| interval      | 1             |    no     |
