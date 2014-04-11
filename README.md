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
    </source>

You also need to enable the nginx_status page in your nginx configuration, see the following link for more details:

http://wiki.nginx.org/HttpStubStatusModule

