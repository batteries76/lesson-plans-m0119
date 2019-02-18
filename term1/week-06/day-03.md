# Day 03 — Rails migrations and model validations
## Outcomes
Students understand the concept of migrations in Rails and can run the scripts that allow them to create data models for Rails as well as place validations on the models

## On successful completion of this unit students will be able to:
- generate a table using a migration
- inspect the table using rails console
- pull or inject data from a database

## Guided instructions
- generate a table ```rails generate model Product name price decimal```
- inspect & discuss migration files ```db/migrations```
- run a migration ```rails db:migrate```
- open rails console ```rails console```
- manipulate & view data in table using model ```Product.all``` in rails console
- add a column to a table ```rails generate migration addDescriptionToProduct description:text```
- add validations to a model
- test validations in rails console
example
```ruby
class Person < ApplicationRecord
  validates :name, presence: true, length: { minimum: 3 }
end

# rails console
person = Person.new
person.valid? # => false
person.errors.size # => 2
 
person = Person.new(name: "Andrea", email: "andrea@example.com")
person.valid? # => true
person.errors.size # => 0
```
- discuss rails callbacks

## Resources
- [Active Record Migrations](http://guides.rubyonrails.org/active_record_migrations.html)
- [Model Validations](http://guides.rubyonrails.org/active_record_validations.html)
- [Model callbacks](http://guides.rubyonrails.org/active_record_callbacks.html)