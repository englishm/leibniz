# Leibniz

Leibniz is simple utility which provides the ability to launch
infrastructure using Test Kitchen, and run acceptance tests against
that infrastructure.  It is designed to be used as part of a set of
Cucumber / Gherkin features.

## Installation

Add this line to your application's Gemfile:

    gem 'leibniz'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install leibniz

## Usage

### Getting Started

Leibniz takes the view that acceptance testing of infrastructure
should be performed from the outside in, and make assertions from the
perspective of an external user consuming the delivered
infrastructure.

To get started, you will need to write some features and some steps.
Depending on how you build your infrastructure (at present the assumed
approach is Berkshelf and wrapper cookbooks, but there's no reason why
it wouldn't work with Librarian-chef, or some other approach).

#### Using Berkshelf

Assuming you have Berkshelf installed, you can use the in-built
cookbook generator to create your wrapper cookbook.  The alternative
is to create a cookbook directory, or use knife to create a cookbook,
and then add 'berkshelf' to a Gemfile, and run bundle install, followed by berks init.

Either way, once you have a cookbook which has been 'berksified' you
will have something that looks like this:



## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
