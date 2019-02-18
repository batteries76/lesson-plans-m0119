# Day 04 — Database design, Entity Relationship Diagram (ERDs), Object Relational Mapping (ORM), SQL & SETS
## Outcomes
Students to get a better understanding of good database design.
Students to be introduced to SQL language. ORM explained. Discrete maths sets further introduction.

## On successful completion of this unit students will be able to:
- design a relational database
- manipulate a sql table
- make basic sql queries
- interact with a SQL like database using an ORM with Ruby
- use sets math to evaluate sets

## Guided instructions

### ORM, SQL, ERD
- Show students poor database structure via exercise:
```
Open an Excel spreadsheet
Explain that most companies keep track of clients, products and services via a spreadsheet.
Demonstrate common mistakes like bad dates, bad ids, missing references, missing addresses, duplicate names, duplicate details, copy and paste mistakes, data deletion and verbose information vs no information.
Explain how businesses structure their data using a database like sql (primary keys, foreign keys etc)
```
- Whiteboard a typical Entity Relationship Diagram (ERD) of a relational database
- ERD Group activity:
```
Have students split into groups of 4/5
Have students choose a business model - e.g. booking agency, cafe, online shop etc
Have students draw on large sheets of paper a relation model of their chosen business
Have each team present
Discuss each teams mistakes or successes in front of the class
```
- discuss [dbdesigner.net](https://dbdesigner.net/)
- demonstrate student ERD into dbdesigner.net
- discuss Structured Query Language (SQL)
- demonstrate SQL via [w3schools](https://www.w3schools.com/sql/)
- discuss the different SQL databases (postgres, MS SQL, sqlite)
- discuss ORM
- demonstrate ORM using sequel gem in a ruby file
    - create a project directory (example-orm)
    - install sqlite ```brew install sqlite```
    - create a main.rb file
    - create a gemfile and add sequel gem ```bundle init```
    - require in sequel gem into main.rb
    - run sqlite database using command line
    - establish connection to sqlite database using sequel gem
    - create a migration.rb file
    - generate a connection to the database in migration.rb
    - generate a SQL table using migration file
    - seed data into the SQL table using a seed.rb file
    - query the table in the main.rb file and print to screen

### Sets Math

￼```
 
 ￼universal set (all the elements)

Empty set (∅ symbol for empty set or if no sets intersect)
Y = {1,2}
Z = {3, 4}

Y ∩ Z = ∅
or Y  ∩ Z = { }

X = { } 
or X =  ∅

UNIONS

A = {1, 2, 3}
B = {1, 3, 4, 6}

Elements in both sets (∩ intersection symbol)
A ∩ B = {1 , 3}

All elements in both sets (∪ union symbol)
A ∪ B = { 1, 2, 3, 4, 6 }

Element is in set B (∈ is in set)
1 ∈ B

Element is NOT in set B (∉ not in set symbol)
2 ∉ B

Number of elements in set B (n symbol for number of elements)
n(B) = 4

Number of elements in set A (cardinal)
n(A) = 3

Is A set equal the number of elements as B (A = 3, B = 4 so no)
A ≠ B 
A = B //not true

Everything NOT in A (~ compliment symbol or you can use ‘ symbol e.g. A‘ )
~A = { 4, 6 }
~B = { 2 }  

SUBSETS

A = {1,2,3,4,5}
B = {4,5}
C = {6, 7, 8}

B is a sub set of A  or every element is present in A (⊆ subset symbol)
B ⊆ A

IF both sets are the same either can be a subset, you’re basically asking the question IS it a subset

B is a proper subset of A as it has less symbols (⊂ proper subset)
B ⊂ A 

Opposite way around A is a Proper set of set A (⊃ superset set symbol)
A ⊃ B

B is not a proper set of A  (⊅ not superset symbol)
B ⊅ A

C is NOT a subset of A (⊄ not a subset symbol)
C ⊄ A


POWER SET
A = {1, 2, 3}

All possible subsets for A
{}, {1}, {2}, {3}, {1, 2}, {1, 3}, {2, 3}, {1, 2, 3}

so powerset 
p(A) = 8


A better way to work that out is (smarter way)

Get the cardinal
p(A) = 3 

then 2 to the power of cardinal result
2 power of 3 = 8

mathy version
n(p(A)) = 2 x 
```


## Resources
- [postgres](https://www.postgresql.org/)
- [sqlite](https://sqlite.org/index.html)
- [Microsoft Server SQL](https://www.microsoft.com/en-us/sql-server)
- [sequel gem](https://github.com/jeremyevans/sequel)