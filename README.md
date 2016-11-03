Spree Look Book
=============

 A lookbook can be described as "fashion diaries" because fashion bloggers are constantly updating them on a daily or weekly basis. This gives customers/viewers ideas on how to style outfits, or to show what the latest fashions are. Lookbooks can be created from admin interface by adding a group of different products(For example: A shirt, pants, shoes, and so on..), with images.

## Installation

1. Add this extension to your Gemfile with this line:
  ```ruby
  gem 'spree_look_book', github: 'askl56/spree_look_book', branch: '3-1-stable'
  ```

  The `branch` option is important: it must match the version of Spree you're using.
  For example, use `3-1-stable` if you're using Spree `3-1-stable` or any `3.1.x` version.

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Copy & run migrations
  ```ruby
  bundle exec rails g spree_look_book:install
  ```

4. Restart your server

  If your server was running, restart it so that it can find the assets properly.

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_look_book/factories'
```


## Contributing

If you'd like to contribute, please take a look at the
[instructions](CONTRIBUTING.md) for installing dependencies and crafting a good
pull request.

Copyright (c) 2016 Andrew Scott, released under the New BSD License
