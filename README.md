# Rails Commands

A collection of useful Ruby on Rails CLI commands for those learning and new to Ruby on Rails.

## New Rails App

To create a new rails app:

```
rails generate new app_name
```

To install the `rails` gem use the following command:

```
gem install rails
```

If you plan to use `rspec` to test your new rails app, then it's best to create a new rails app without the redundant ruby tests folder. The command to do this:

```
rails generate new app_name --skip-test-unit
```

To learn the other options available for the `rails new` command use the following command:

```
rails new --help
```

## Creating Models

To create a new rails model use the following command:

```
rails generate model ModelName [field[:type] field[:type]]
```

As always stick to rails conventions by ensuring the name of your model uses singular tense. Also ensure that the name of your model uses Camel casing (e.g. Account, Order, LineItem etc). When generating a model we need to provide the names of the fields/attributes of our model and it's type.

Rails support the following types:

* integer
* primary_key
* decimal
* float
* boolean
* binary
* string
* text
* date
* time
* datetime
* timestamp

### Running Migrations

When a model is creating a corresponding migration is created in the folder db/migrations. Running a migration will build the models supporting table. The migration can be run with the following command:

```
rake db:migrate
```

## Creating Migrations

Sometimes a migration is required to amend a tables/models definition. Such a migration can be created with the following command:

```
rails generate migration migration_name
```

A migration can be run with the following command:

```
rake db:migrate
```

For more information on creating rails migrations please consult the following [guide](http://edgeguides.rubyonrails.org/active_record_migrations.html)

## Creating Controllers

Rails provides a generator for creating controllers. The format of the command is as follows:

```
rails generate controller ControllerName [action action]
```

In rails a controller's name is plural (e.g. Accounts, Users etc) by convention. When generating a controller the name of the actions can be provided an optional argument, each action's name is separated by a space.

This generator will also generate test place holders for the corresponding controller. To stop the generator from generating such tests use the option --no-test-framework option. So to generate a controller without tests use the following command:

```
rails generate controller ControllerName [action action] --no-test-framework
```

## Starting/Stopping A Server

To start a rails server use the following command:

```
rails server
```

To start the server on a port other than port 3000 use the following command:

```
rails server -p 4000
```

Stopping a rails server is as simple as using `ctrl c`.

## Access the rails console

The rails console can be accessed with the following command:

```
rails console
```
