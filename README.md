# ImageFetcher

Welcome to your new gem! In this directory, you'll find the files you need to be able to package up your Ruby library into a gem. Put your Ruby code in the file `lib/image_fetcher`. To experiment with that code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'image_fetcher'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install image_fetcher

## Usage

-   Add a directory `/images`
-   Add a file with image urls (e.g images/list.txt)
-   Run `ruby -Ilib ./bin/image_fetcher images/list.txt`

## Structure & Classes

- parser
  - reads file
  - logs out error if read fails
  - loops over file lines
  - prints image index
  - calls downloader with the url/line

- downloader
  - takes url as input
  - downloads image from url using the Down gem
  - logs out error if download fails
  - logs out success if download succeeds

- logger
  - logs out success, error, warning, info messages
  
## Todo

- Fillout test cases

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/image_fetcher.

