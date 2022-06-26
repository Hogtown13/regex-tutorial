# Regex Tutorial 

With this tutorial I will explain what a Regex is and how its constructed.  

## Summary

Regex, short for regular expression, is a string of text used for creating a pattern that helps 
match, locate, and manage text.

Here is an example of a Regex Matching an HTML Tag –  /^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/ 




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
/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/ 

The ^ and $ are anchors used to start and end our string expression

### Quantifiers

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.
The + and * are quantifiers in this expression, the + is used to match one or more times of the preceding element in this case [a-z] and [^<].
The * is used to match zero or more times of its preceding element, in this case ([^<]+).

### OR Operator

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

The | operator matches elements before or after it, in this case > OR \s .

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
