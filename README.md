# Node.js Compiler

Compiler for Node.js which compiles your app into a single executable.

http://nodec.enclose.io

[![Linux and Mac OS X Build Status](https://travis-ci.org/enclose-io/node-compiler.svg?branch=master)](https://travis-ci.org/enclose-io/node-compiler)
[![Windows Build status](https://ci.appveyor.com/api/projects/status/f4x3bq5hub3uu3ys/branch/master?svg=true)](https://ci.appveyor.com/project/pmq20/node-compiler/branch/master)
[![Gem Version](https://badge.fury.io/rb/node-compiler.svg)](https://badge.fury.io/rb/node-compiler)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'node-compiler'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install node-compiler


## Usage

    nodec [module_name] [module_version] [bin_name] [output_path]

## Example

    nodec coffee-script 1.11.1 coffee coffee-1.11.1-darwin-x64

Then the compiled product will be located at `./coffee-1.11.1-darwin-x64`, ready to be distributed.

## Optional Environment Variables

* `ENCLOSE_IO_KEEP_WORK_DIR`
* `ENCLOSE_IO_CONFIGURE_ARGS`
* `ENCLOSE_IO_MAKE_ARGS`
* `ENCLOSE_IO_VCBUILD_ARGS`
* `ENCLOSE_IO_NPM`
* `ENCLOSE_IO_NPM_INSTALL_ARGS`
* `npm_config_registry`

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. Or without installing, run `bundle exec nodec` from the root of your project directory.

To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/enclose-io/node-compiler.

## Contributors

* [pmq20](https://github.com/pmq20) - **Minqi Pan** &lt;pmq2001@gmail.com&gt;
* [ibigbug](https://github.com/ibigbug) - **Yuwei Ba** &lt;akabyw@gmail.com&gt;

## License

Copyright (c) 2016 Node.js Compiler contributors, under terms of the [MIT License](http://opensource.org/licenses/MIT).
