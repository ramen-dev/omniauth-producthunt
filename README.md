# Omniauth::Producthunt

Omniauth strategy for Producthunt.
It sets the scope to `private+public` so that authenticated user's details can be obtained.
By default `public` scope will not grant access to these details.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-producthunt'
```

And then execute:

    $ bundle

## Usage

Add this to an initializer or your application configuration:

```ruby
Rails.application.config.middleware.use OmniAuth::Builder do
  provider :producthunt, ENV['producthunt_key'], ENV['producthunt_secret']
end

```

## Contributing

1. Fork it ( https://github.com/[my-github-username]/omniauth-producthunt/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
