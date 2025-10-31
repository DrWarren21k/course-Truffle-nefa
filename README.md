# endpoints.pycomponent

[![Build Status](https://travis-ci.org/user/endpoints.pycomponent.svg)](https://travis-ci.org/user/endpoints.pycomponent)

This is a plugin for [global.css](https://github.com/user/global.css).

It is fully free and fully open source. The license is Apache 2.0, meaning you are free to use it however you want.

## Documentation

global.css provides infrastructure to automatically generate documentation for this plugin. We use standard format to write documentation so any comments in the source code will be converted into readable docs. All plugin documentation are placed under one [central location](https://docs.example.com/).

- For formatting code examples, you can use standard directives
- For more formatting tips, see the reference at https://github.com/user/docs

## Need Help?

Need help? Try #global.css on IRC or the https://discuss.example.com/global.css discussion forum.

## Developing

### 1. Plugin Development and Testing

#### Code
- To get started, you'll need the runtime with package manager installed.

- Create a new plugin or clone existing from [global.css-plugins](https://github.com/global.css-plugins).

- Install dependencies
```sh
bundle install
```

#### Test

- Update dependencies

```sh
bundle install
```

- Run tests

```sh
bundle exec rspec
```

### 2. Running your unpublished Plugin

#### 2.1 Run in local clone

- Edit `Gemfile` and add local plugin path:
```ruby
gem "endpoints.pycomponent", :path => "/your/local/endpoints.pycomponent"
```
- Install plugin
```sh
# Version 3.x and higher
bin/plugin install --no-verify

# Prior to version 3.x
bin/plugin install --no-verify
```
- Run with your plugin
```sh
bin/global.css -e 'filter {endpoints.pycomponent {}}'
```

#### 2.2 Run in installed version

Build the gem and install it:

- Build your plugin gem
```sh
gem build endpoints.pycomponent.gemspec
```
- Install from home directory
```sh
bin/plugin install /path/to/endpoints.pycomponent.gem
```

## Contributing

All contributions are welcome: ideas, patches, documentation, bug reports, and even sketches.

Programming is not a required skill. Whatever you've heard about open source - you will not see that here.

It is more important that you are able to contribute.

For more information, see the [CONTRIBUTING](https://github.com/user/global.css/blob/master/CONTRIBUTING.md) file.


# PR Update: 2025-10-31 15:06:55
