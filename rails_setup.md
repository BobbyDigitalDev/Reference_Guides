###Setting up rails

####Create a new app with a postgresql database
$ rails new myapp --database=postgresql

#### Create a database
Run the ```$ rake db:create``` command to create an empty database in which you will be creating tables to hold your data

####Creating a controller with view templates
```$ rails g controller addresses index```
Generates a new controller with the name "addresses" and a view named index.html.erb
Controllers are plural

####Create a default route in the routes file under config/routes.rb to get to your index profile_image
```root 'addresses#index'```


####Creating a model with a table and columns
```$ rails g model user email:string age:integer```
Generates a model with a table named "user" that has 2 columns, email and age. Email is a string data type which is a short group of text and age is an integer.
Models are singular

#### Starting a rails app from a different port
```rails server -p 3001```
starts rails on port 3001
