# Apple::Music

Apple::Music acts as an abstraction for interacting with Apple Music's API.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'apple-music', git: 'https://github.com/assemble-inc/apple-music-api'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install apple-music

Create a `$PROJECT_ROOT/.env` file with your API authentication information:

    APPLE_MUSIC_SECRET_KEY="-----BEGIN PRIVATE KEY-----\nabcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789/+\n-----END PRIVATE KEY-----"
    APPLE_MUSIC_KEY_ID=ABCDEFG012
    APPLE_MUSIC_TEAM_ID=HIJKLMN345

Note that the underlying libraries are _very_ sensitive to how `APPLE_MUSIC_SECRET_KEY` is formatted.

Test the configuration by verifying `rake load_client` exits silently without error.

## Usage

TODO: Write usage instructions here

## Development

+ install dependencies `bin/setup`
+ run tests `rake spec`
+ console `rake console`

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Contact Chris (chris [at] weassemble.com)
Melissa (melissa [at] weassemble.com)

## stuff

+ run `client = load_client` to easily create
+ run `reload!` to reload code
