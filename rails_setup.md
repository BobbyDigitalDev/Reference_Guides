###Setting up rails

####Create a new app with a postgresql database
$ rails new myapp --database=postgresql

####Creating a model with a table and columns
$ rails g model user email:string age:integer


####Creating a controller with view templates
```$ generate controller Greetings hello```
Generates a new controller with the name "Greetings" and a view named hello.html.erb