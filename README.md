Rails Devise With Intercom
================

To start testing your Intercom app on this sample app you need to clone this repo:

```shell
  git clone https://github.com/Skaelv/rails-devise-with-intercom
  cd rails-devise-with-intercom
  bundle install
```

In the `config/initializers/intercom.rb` file replace the following line with your Intercom app_id:
```ruby
  config.app_id = ENV["INTERCOM_APP_ID"] || "<your-app-id>"
```

And run the ruby server :
```shell
rails s
```

If everything is fine you should see the Intercom messenger appear right away.

Troubleshooting
----------------

If the Intercom messenger doesn't show up. Check that you have registered to any Intercom product.
If you didn't subscribe to Acquire but to other products, try to sign-up to the sample app and see if the messenger appears once you are logged-in.
