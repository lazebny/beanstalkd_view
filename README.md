[![Build Status](https://secure.travis-ci.org/denniskuczynski/beanstalkd_view.png?branch=master)](http://travis-ci.org/denniskuczynski/beanstalkd_view)

A Sinatra app to view/manage beanstalkd queues that can be embedded in a Rails app similar to what's available in Resque.

To use, include the gem:

gem beanstalkd_view

And in your routes.rb file:

mount BeanstalkdView::Server, :at => "/beanstalkd"

You can then browse to your application path to view information about your beanstalkd tubes, i.e.
http://127.0.0.1:3000/beanstalkd
