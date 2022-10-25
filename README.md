# Regex Tutorial for Matching an Email 

This tutorial will explain how a regex functions by breaking down each part of the expression and describing what it does.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

In this tutorail, we will be looking at the following regex expression and how it helps us validate or match an email:  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
The family of regex tokens that don't match any characters but make a claim about the string or the matching procedure includes anchors. Anchors claim that the engine is currently located in the string at a location that is known to exist, such as the start of the string or the end of a line.
#### Anchors in email validation: 
- [^,$]
- - [^ : starting position]
- - [$ : ending position]

### Quantifiers
The number of instances of the previous element—which could be a character, a group, or a character class—that must be present in the input string for a match to take place is specified by a quantifier. They also choose whether a regex will try a lazy or greedy match.

### Character Classes
Character Classes correspond to a certain collection of characters. You can define distinct sets or choose from predefined classes. A sizable set of character classes can also be mixed.
#### Character classes in email validation: 
- [a-z, 0-9, /d, /., @]

### Flags
Six optional flags in regular expressions enable features like global and case-insensitive searches. These flags, which are a component of the regular expression, can be used individually or collectively in any combination.
#### 

### Grouping and Capturing


### Bracket Expressions


### Greedy and Lazy Match


### Boundaries


### Back-references


### Look-ahead and Look-behind


## Author


A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)