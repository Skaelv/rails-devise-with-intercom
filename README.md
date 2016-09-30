Rails Devise With Intercom
================

To start testing your Intercom app on this sample app you need to clone this repo:

```shell
  git clone https://github.com/Skaelv/rails-devise-with-intercom
  cd rails-devise-with-intercom
  bundle install
  rake db:migrate
```

In the `config/initializers/intercom.rb` file replace the following line with your Intercom app_id:
```ruby
  config.app_id = ENV["INTERCOM_APP_ID"] || "<your-app-id>"
```

And run the ruby server :
```shell
rails s
```

If you want to use this repo to contribute/test [`intercom-rails`](https://github.com?intercom/intercom-rails) you can just modify the Gemfile as follow:

```ruby
gem 'intercom-rails', :git => 'https://github.com/intercom/intercom-rails.git', :ref => '0eec4'
gem 'intercom-rails', :git => 'https://github.com/intercom/intercom-rails.git', :branch => 'new-feature-branch'
```


If everything is fine you should see the Intercom messenger appear right away.

Troubleshooting
----------------

If the Intercom messenger doesn't show up. Check that you have registered to any Intercom product.
If you didn't subscribe to Acquire but to other products, try to sign-up to the sample app and see if the messenger appears once you are logged-in.
