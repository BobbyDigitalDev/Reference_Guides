###Setting up rails

####Create a new app with a postgresql database
$ rails new myapp --database=postgresql

####Creating a model with a table and columns
```$ rails g model user email:string age:integer```
Generates a model with a table named "user" that has 2 columns, email and age. Email is a string data type which is a short group of text and age is an integer.


####Creating a controller with view templates
```$ generate controller Greetings hello```
Generates a new controller with the name "Greetings" and a view named hello.html.erb