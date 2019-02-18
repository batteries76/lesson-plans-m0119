# Day 04 — Arrays, if/else, loops
## Outcomes
Students have a basic understanding of arrays, ranges, truth statements, operators, switch statement, ternary operation (expressions) and loops


## On successful completion of this unit students will be able to:
- manipulate an array
- have a basic understanding of ranges
- write an if statement with else
- write a case/switch statement
- write a ternary expression
- write loops
- loop an array

## Guided instructions

### Arrays
- create an array
- return element of an array
- push and element to an array
- pop an element off an array
- concatenate two arrays ```.concat```
- split a string into an array ```.split```
- join an array into a string ```.join```
- length of array ```.length```
- fetch an element of an array ```.fetch```
- element included in array ```.include?```
- insert element at index ```.insert```
- reverse elements ```.reverse```
- shuffle elements ```.shuffle```

# Ranges
- discuss ranges
- show doc page
Examples:
```ruby
(1..5).each {|num| puts "#{num}\n"}

case 79
    when 1..50   then   print "low\n"
    when 51..75  then   print "medium\n"
    when 76..100 then   print "high\n"
end
```

### Booleans data type 
NOTE: good time to introduce truth tables at the end
- Talk about true and false
- code ```true```
- code ```false```
- equal to comparison operator ```==```
- not equal to comparison operator ```!=```
- greater than operator ```>```
- less than operator ```<```
- greater than or equal to ```>=```
- less than or equal to ```<=```

### if/else statements (conditionals)
- write an if statement
- add an else to the if statement
- add an elsif to the if statement

### Logical operators
Note: good to get into AND, OR, XOR discrete maths
- AND operator ```&&```
- OR operator ```||```
- NOT operator ```!```

### Case statement
- ruby switch statement with at least 3 cases & an else

### Ternary expression
- write a ternary expression ```puts x ? 'is true' : 'is false'```

### Loops
- discuss loops
- discuss infinite loops
- while loop ```while```
- do block ```do```
```ruby
# optional advanced example of using a do block with a ruby method

def say_hello
    yield # do block will be run here
end
 
say_hello { puts "hello world" } # do block passed to method
```
- begin while ```begin while```
- until loop ```until```
- for in loop ```for in```
- break out of loop ```break```

### Loop arrays
- learn about looping arrays the better way ```.each```
- each with index ```.each_with_index```

## Resources
- [Array](https://ruby-doc.org/core-2.5.0/Array.html)
- [Range](https://ruby-doc.org/core-2.5.0/Range.html)
- [Control Expressions & loops](https://docs.ruby-lang.org/en/2.5.0/syntax/control_expressions_rdoc.html)

## Examples
- [Boolean and Logical Operator Test](https://github.com/GretchS/lesson-content/blob/master/test-questions/boolean-operators.rb)

## DISCRETE MATHS — LOGIC
Truth tables (no binary truth table)
AND, OR, XOR (exclusive or)

## Challenges

## Units
- Array
- Control Structures
- Methods
- Blocks
- Structure
- Ranges
- Maths Logic
