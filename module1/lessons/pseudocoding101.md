
From http://backend.turing.io/module1/lessons/pseudocoding101

# Learning Goals
  
Be able to define the term pseudocode and algorithm

> Algorithm - Process (somewhat like a recipe) that tells the computer how to accomplish a task

> Pseudocode - Informal high level description of the algorithm

Be able to use pseudocode to describe the flow of an algorithm’s implementation

# Part 1 - Writing

1. Take one lace in your left hand
2. Take the other lace in your right hand
3. Move the right lace over the left lace, then under the left lace
4. Pull until tight
5. Wrap the lace in your left hand around your right thumb making a loop
6. Hold both ends of the loop in your left hand
7. With the right lace, go above the loop, then under the loop
8. Push the right lace through the hole formed by 7, making a second loop
9. Pull the two loops until tight

# An Iterative Process

A generalized process for solving technical problems:

1. How will you know when the problem is solved? (Identify the big-picture goal)
2. How do you want to use the software? (Identify the “interface”)
3. What’s the (next-)most trivial possible case? (Identify the next small-picture goal)
4. How do we achieve this goal? (Sketch an algorithm using pseudocode)
5. Implement it (do programming)
6. Is the whole problem (from step 1) solved? If not, return to 3.

# Common Words

## Problem:

I have a text document and want to know “What are the three most common words in the text?”

Extension: Let’s exclude the following: I, you, he, she, it, we, they, they, a, an.

1. I will see "The three most common words are: ______, ______ and _______"
2. ./count_words path/to/file.txt
3. Work with a file with only three words on a single line
4. 

```
Open the file
Read the line
Split the line up into words
Count how many times each word occurs
Output the most common words
```

3. Work with a file with the same three words on two lines (each word occurs twice, once per line)

4. Same

3. Work with a file with three lines, the third line is a fourth word that doesn't occur in the first two lines

4. Same, but output should not include the fourth word you added

Extension would not count the word if it was in the exclusion list

# Odds & Evens

## Problem:

I have a file with 100 numbers. I want to create two new files: one with all the odds and one with all the evens.

1. I end up with two files "odd.txt" and "even.txt".  Odd.txt should only have odd numbers, even.txt should only have even numbers.

2. ./split_odd_and_even path/to/numbers.txt

3. Work with a file that only has one odd number as input
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into an number
  If the number is odd, write it to odd.txt
  If the number is even, write it to even.txt
```

Verify the file odd.txt has one line (the odd number), and even.txt has no lines.

3. Work with a file that only has two odd numbers as input
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into an number
  If the number is odd, write it to odd.txt
  If the number is even, write it to even.txt
```

Verify the file odd.txt has two lines (the odd numbers), and even.txt has no lines.

3. Work with a file that has two odd numbers and one even number as input
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into an number
  If the number is odd, write it to odd.txt
  If the number is even, write it to even.txt
```

Verify the file odd.txt has two lines (the odd numbers), and even.txt has one lines (the even number).

Extension would need to remember if it's seen a number before writing it to either even.txt or odd.txt.

# Lats & Longs

## Problem:

I have a file with 100 latitude/longitude pairs. Find the point that’s closest to the north pole.

1. The output says "Point _____, ______ is closest to the north pole"
2. ./find_closest_point path/to/pairs.txt

3. Work with a file that has one point (0, 0)
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into two numbers
  If Min is nil
    Set Min distance to the first number (degrees latitude)
    Set closest_point to first_number, second_number
  else if Min > the first number
    Set Min to the first number
    Set closest_point to first_number, second_number
Output "The closest point is closest_point
```

3. Work with a file that has two points (1, 0) and (5, 0)
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into two numbers
  If Min is nil
    Set Min distance to the first number (degrees latitude)
    Set closest_point to first_number, second_number
  else if Min > the first number
    Set Min to the first number
    Set closest_point to first_number, second_number
Output "The closest point is closest_point
```
Verify output is 1, 0

3. Work with a file that has three points (1, 0), (5, 0) and (3, 2)
4. 

```
Open the file
While there's more lines in the file:
  Read a line
  Parse the line into two numbers
  If Min is nil
    Set Min distance to the first number (degrees latitude)
    Set closest_point to first_number, second_number
  else if Min > the first number
    Set Min to the first number
    Set closest_point to first_number, second_number
Output "The closest point is closest_point
```
Verify output is 1, 0

Extension: Find the lat/long of magnetic north and use that instead of 0, 0

