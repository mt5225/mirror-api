# Mirror::Api

Mirror API client

## Installation

Add this line to your application's Gemfile:

    gem 'mirror-api'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install mirror-api

## Usage

``` ruby

# Insert a simple text item - https://developers.google.com/glass/timeline#inserting_a_simple_timeline_item
timeline_api = Mirror::Api::Timeline.new({:token => access_token})
item = timeline_api.post({:text => "Hello Word"})

# Inserting an item with reply actions - https://developers.google.com/glass/timeline#user_interaction_with_menu_items
item2 = timeline_api.post({:text => "Hello Word", :menu_items => [{:action => "REPLY"}]})

```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
