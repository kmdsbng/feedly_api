feedly_api
==========
[![Coverage Status](https://coveralls.io/repos/Myuzu/feedly_api/badge.png)](https://coveralls.io/r/Myuzu/feedly_api) [![Build Status](https://travis-ci.org/Myuzu/feedly_api.png?branch=master)](https://travis-ci.org/Myuzu/feedly_api) [![Code Climate](https://codeclimate.com/github/Myuzu/feedly_api.png)](https://codeclimate.com/github/Myuzu/feedly_api) [![Dependency Status](https://gemnasium.com/Myuzu/feedly_api.png)](https://gemnasium.com/Myuzu/feedly_api) [![Gem Version](https://badge.fury.io/rb/feedly_api.png)](http://badge.fury.io/rb/feedly_api)

Early unofficial Feedly API with no external dependencies

## Limitations
* no auth for now
* get methods only
* continuation not implemented

## Usage

```ruby
# Create client for API requests; OAuth token optional
@client = FeedlyApi::Client.new
# Create Feed object for specific feed id
@feed = @client.feed('feed/https://www.eff.org/rss/updates.xml')
# Get array of feed items hashes
@feed.items
# Pass params to get more or less items
@feed.items(count: 50)
```

## Supported Ruby Versions

feedly_api is tested under 1.9.3, 2.0.0, JRuby (1.9 mode), and Rubinius (1.9 mode).

## License

Apache License, Version 2.0
