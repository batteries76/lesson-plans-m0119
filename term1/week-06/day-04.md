# Day 04 — Rails model associations
## Outcomes
Students to connect records in tables through database relationships using the built in Rails model associations

## On successful completion of this unit students will be able to:
- create a table
- create a related table of records
- foreign keys in Rails
- associate one table with another
- pull associated records of a table from a separate table's record

## Guided instructions
- discuss types of associations
```
belongs_to
has_one
has_many
has_many :through
has_one :through
has_and_belongs_to_many
```
- discuss foreign keys, primary keys
- create a brands model ```rails g model Brands name```
- create a products model ```rails g model Product name price:decimal description:text brand:references```
- add associations to model
- open rails console ```rails console```
- create a brand and add it to a variable
- create a product with a brand (using variable)
- repeat for several products with different brand ids as the foreign key
- TODO: finish this day

[Association basics](http://guides.rubyonrails.org/association_basics.html)