###Heroku Gems for Rails
####Add
```rails_12factor``` gem to your ```Gemfile```

At the end of Gemfile add:
gem ```gem 'rails_12factor', group: :production```

Then run:
```$ bundle```

###Specify Ruby version in app

At the end of Gemfile add:
```ruby "2.2.2"```
To check the installed version type the following in the command line ```$ ruby -v```
Then run:
```$ bundle```

_git add and commit_

###Deploy your application to Heroku
####Log into your heroku account

Create your heroku app connection
type
```$ heroku create appname```

Deploy your app up to heroku
 ```$ git push heroku master```

 Migrate your database
 ```$ heroku run rake db:migrate```

 Make sure you have one dyno running
 ```$ heroku ps:scale web=1```

Check the state of the app’s dynos
```$ heroku ps```

To launch your app from the CLI
```$ heroku open```

View the logs
```$ heroku logs```

Access the heroku console
```$ heroku run rails console```

Running rake
```$ heroku run rake db:migrate```

Adding a custom domain
First confirm your heroku account by adding a credit card number to you profile.
```heroku domains:add www.example.com```

Check on the status of your domain trainsfer by digging the name
```$ dig example.com +nostats +nocomments +nocmd```
You will see that the domain is routed to the heroko repo can take several hours depending on the settings
