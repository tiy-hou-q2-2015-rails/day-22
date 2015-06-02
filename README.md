Day 22 - Rails Active Record
====

tuesday: joins / AR
wednesday: 

Challenge
--------

### Part 1

Assuming standard Rails conventions, create a "CREATE TABLE" statement for
pandas. Pandas have a name, gender (M/F), belong to a zoo, weight in kilograms, and have a
personality where zoo keepers describe their traits/likes/dislikes.

Don't forget the Primary Key and the CreatedAt/UpdatedAt!

### Part 2

Zoo keepers would like to find the two largest pandas, one male and one female.
Please write the SQL queries to find that information.

Today
-----

1. Challenge
1. Multiple Tables
1. Joins
1. ActiveRecord `where/find_by/save`
1. CreatingTables, re-running migrations

Assignment
-------


1. Create a Bloging Rails Application
1. Your Post should have a `title`, `body`
1. You should have a proper "db/seeds.rb" that populated your title and posts
   when you run `rake db:seed`
1. When you go to "http://localhost:3000" it should list all posts (title and
   truncated body)
1. You should click on the title and go to "http://localhost:3000/posts/:id" and
   display the title and body
1. Add `published_on` to the Post using a migration
1. Only show pubished posts



Notes
-----

How to create a Rails app, with a database and model.

```
rails new pancakes
cd pancakes
rake db:create
rails generate model pancake name
rake db:migrate
rails g controller Flour
rails g migration AddPhotoToPancake
echo 'edit the migration in db/migrations and add field names'
rake db:migrate
echo 'Now you edit the db/seeds.rb and Pancake.create'
rake db:seed
rails s
```
