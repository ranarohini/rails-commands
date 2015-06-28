Rails Commands
==============

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

To learn what the other options are for the `rails new` command use the following command:

```
rails new --help
```

## Creating Models

TODO:

## Creating Migrations

TODO:

## Creating Controllers

TODO:

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
