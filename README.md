# Regex Tutorial for Matching an Email 

This tutorial will explain how a regex functions by breaking down each part of the expression and describing what it does.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

In this tutorail, we will be looking at the following regex expression and how it helps us validate or match an email:  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The family of regex tokens that don't match any characters but make a claim about the string or the matching procedure includes anchors. Anchors claim that the engine is currently located in the string at a location that is known to exist, such as the start of the string or the end of a line.
- [^,$] symbols are used in our email validation expression
  - ^ : starting position
  - $ : ending position
Example in email validation: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ <-- You can see the "^" at the beginning of the check and the "$" at the end of the check 
### Quantifiers
The number of instances of the previous element—which could be a character, a group, or a character class—that must be present in the input string for a match to take place is specified by a quantifier. They also choose whether a regex will try a lazy or greedy match.
- '+' , {2,6} quantifiers are used in our email validation
  - '+' : matches one or more of the previous expression
  - {2,6} : the value of the previous token
  
Example in email validation: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ <-- You can see the + allows the characters from a to z (a-z), 0 to 9 (0-9), and an underscore. 

Example in email validation: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ <-- You can see the {2,6} being used to define how many of (a-z\.) it can use before the end of the email  
### Character Classes
Character Classes correspond to a certain collection of characters. You can define distinct sets or choose from predefined classes. A sizable set of character classes can also be mixed.
- In this email we are using the following character classes: a-z, 0-9, /., @
  - a-z is any character from a to z as discussed before 
  - 0-9 is any number from 0 to 9
  - /. a forward slash is considered an escape character. In this case we are using it for the period (.com)
Example in email validation: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ <-- You can see all the quantifiers mentioned above in this example 

### Grouping and Capturing
To regard a set of characters as a single entity they must be captured. They are made by putting the characters inside parenthesis that will form the group.
- For example: ibrahim@gmail.com
  - "ibrahim" is the first group
  - "gmail" is the second group 
  - ".com" is the third group 

### Bracket Expressions
Bracket expressions are what seperate lists of classes from each other 
- For example in our regex we have 3 different bracket seperations:  [a-z0-9_\.-], [\da-z\.-], and [a-z\.]

### Greedy and Lazy Match
- There are two types of matching when working with regex: 
  - Greedy: match as many characters as possible
  - Lazy: match as few characters as possible

## Author

My name is Ibrahim and this tutorial was made as part of an assignment for a Fullstack Web Developer Bootcamp. Check out my github! [Ibrahims github](https://github.com/bebo96 "Ibrahim Imran")
