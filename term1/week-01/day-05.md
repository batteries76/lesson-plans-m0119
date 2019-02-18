# Day 05 — Hashes & Ruby test
## Outcomes
Students to know how to manipulate ruby hashes, how they can be used to represent real world objects and a comprehension of symbols and what they represent.

Students to know about datetime, date & time data type / object

## On successful completion of this unit students will be able to:
- manipulate a hash
- setting values in a hash
- accessing values from a hash
- loop a hash ```.each```
- utilize a symbol either in a hash or variable
- can manipulate date/time values in ruby
- can format, convert and compare dates

## Guided instructions

### Hashes & Symbols
- create a hash
- talk about difference between old hash rockets and new way
- discuss hashes representing real world objects
- discuss symbols (dictionary term, history)
- demonstrate hash objects
- explain ```.object_id```
- loop over a hash
- pull values from a hash
- set values in a hash

### Date, DateTime, Time
- create a time ```Time.new```
- manipulate a time
- create a date ```Date.new```
- manipulate a date
- parse a string into a date ```.parse```
- create a datetime ```DateTime.new```
- talk about formatting dates
- stringify a date ```strftime```
- convert datetime to date ```.to_date```
- discuss how a computer stores dates (1 Jan 1970 00:00:00)
- date to UTC (Coordinated Universal Time) ```.utc```
- date to number ```.utc.to_i```
- comparing integer dates

```ruby
require 'time'
date = Time.now.utc.to_i
time = Time.new(1970,1,1,0,0,0,0).utc.to_i
puts time
puts Time.at(time)
```

### Combine everything learnt
- combine arrays, strings, numbers, booleans, hashes, dates, loops and conditionals

### Ruby Test
- on paper written test with Ruby questions

### (optional) Early Introduction to methods
- see week 2 day 1

## DISCRETE MATHS — Sets
Go through a very basic set of numbers explaining uniqueness in a set - use whiteboard. Each element represented as ```∈```

```x = { 1, 2, 3, 4, 5 }```

## Resources
- [Hash](https://ruby-doc.org/core-2.5.0/Hash.html)
- [Symbol](https://ruby-doc.org/core-2.5.0/Symbol.html)
- [Time](https://ruby-doc.org/stdlib-2.5.0/libdoc/date/rdoc/Time.html)
- [Date](https://ruby-doc.org/stdlib-2.5.0/libdoc/date/rdoc/Date.html)
- [DateTime](https://ruby-doc.org/stdlib-2.5.0/libdoc/date/rdoc/DateTime.html)

## Challenges

## Units
- Hashes
- Symbols
- Maths Sets
- Ruby Test
- Methods




