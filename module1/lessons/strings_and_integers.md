From http://backend.turing.io/module1/lessons/strings_and_integers

Learning Goals

# Strings

define “string”

> A string of letters, numbers or symbols contained within double or single quotes

## Practice

Which of the following are valid strings? Why?

1. ’’  # Valid, it's an empty string surrounded by single quotes
2. “123” # Valid, it's the number 123 surrounded by double quotes
3. 123 # Invalid, there are no quotes
4. ”@*#%&” # Valid
5. hello, world! # Invalid, no quotes
6. ‘welcome to Turing’ # Valid
7. ‘987654321.” # Valid
8. “hot chocolate is the best” # Valid

## Substrings

The bracket notation lets you return a specific character.  "hello, world"[0] will return the first letter ('h')

Providing a range of numbers will return a range of the string: "hello, world"[0..4] will return "hello"

Negative numbers in ranges start from the end of the string instead of the beginning.

## Methods on String

`upcase` makes all the letters in the string upper case

Learned about Ruby Documentation (use Dash!)

`delete` Removes all occurrences of the letter from the string

`downcase` Makes all the letters lower case

`empty?` Returns true or false on whether the string is empty or not

`gsub` Replaces all occurrences of a letter/string within a string with a new value

`include?` Returns true or false on whether the string includes the passed in string

`index` Returns the index of the first occurrence of the letter/string within the string

`length` Returns how long the string is

`reverse` Returns a new string in reverse order

`split` Splits a string into an array split on the supplied string

`start_with?` Returns true or false on whether the string starts with the letter/string

`tr` Transposes letters

`upcase` Replaces all lower case letters with upper case letters

`==` Returns true/false if the strings have the same characters (case matters)

## Naming variables

1. always start with a lower case letter or underscore
2. have no spaces
3. Do not contain special characters ($, @, &)

## String style

1. use_snake_case
2. Named after meaning, not contents (`my_name` vs `my_name_string`)
3. aren't abbreviated (don't use `j` or I hurt you)

## Practice

Which of the following are valid strings? Why?

1. `time_machine` # Valid
2. `student_count_integer` # Valid, not good Ruby syntax (mentions the type)
3. `homeworkAssignment` # Valid, not good Ruby syntax (camelCase instead of snake_case)
4. `3_sections` # Invalid, must start with letter or underscore
5. `top_ppl` # Valid, not good Ruby syntax (uses abbreviations)

# Integer

define “integer”

> A whole number (i.e. no decimal portion)
 
Ruby 2.4.0 got rid of Fixnum/Bignum (http://blog.bigbinary.com/2016/11/18/ruby-2-4-unifies-fixnum-and-bignum-into-integer.html)

## Methods on String

`round` Returns the number on Integers, rounds the number to the nearest whole number for floats

`to_f` Converts to a float

`to_i` Converts to an integer (doesn't round, simply drops everything after .)

`to_s` Converts to a String

`floor` Rounds down to nearest whole number

`ceil` Rounds up to nearest whole number

`abs` Returns the positive value of a number (changes negative #'s to positive)

`%` Modulo arithmatic (the remainder)

`==` Compares the two numbers, returns true/false if they're equal

`>` Is the first number greater than the second?

`>=` Is the first number greater than or equal to the second?

`even?` Is the number even? (Doesn't work on floats)

`odd?` Is the number odd? (Doesn't work on floats)

`next` Increments the number by 1 (Doesn't work on floats)

`upto` Loop through the numbers by 1 until reaching the upto number

`times` Loops through number of times

define “float”
assign values to variables using proper naming conventions
use string concatenation with literal strings and variables
use string interpolation with variables
call key methods on strings
call key methods on integers and floats
read Ruby documentation
