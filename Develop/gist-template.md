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
The + and * are quantifiers in this expression. The + is used to match one or more times of the preceding element in this case [a-z]+ and [^<]+.
The * is used to match zero or more times of its preceding element, in this case ([a-z]+)([^<]+)*.

### OR Operator

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

The | operator matches elements before or after it, in this case > OR \s .

### Character Classes

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Character classes or character sets are square brackets [a-z] [^<], they allow you to tell the regex engine to only match characters that are inside the brackets. You can also use hyphens inside of character sets like in our example to give a range of characters to match.

### Flags

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Flags are optional parameters that modifiy the way the regex searches. They use single lowercase letters set after the expression or outside the ending / . There is no flag in our example however if we added a g to the end of our expression it would look like this
(?:>(.*)<\/\1>|\s+\/>)$/g , which stands for globally and allows the expression search for all instances.

### Grouping and Capturing

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

With grouping and capturing we are using ( ) to capture text or characters within them. In our example one of the groupings is ([a-z]+) 
which allows us to group the character class [a-z] with the quantifier + .

### Bracket Expressions

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

bracket expressions are characters enclosed by [ ]. In our example [a-z] and [^<] are used. In the First example we are setting asearch for the letters a through z, in the second example we are setting the search for a negated set that matches any character not in the set and also matching any < character.

### Greedy and Lazy Match

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Greedy is an algorithm that for every position in the string trys to match the pattern at that position, if there's no match then go to the next position. Lazy mode is the opposite of greedy, it is used by adding a ? symbol to a quantifier to repeat the search the fewest times possible. Our expression is Greedy because it does not have a quantifier directly followed by a ? .

### Boundaries

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Boundaries are used like anchors, they give the regex search engine a starting and ending point to check for characters. We do not use them in our regex string. 

### Back-references

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Back-references are used to go back and reference a captured group. In our example our first captured group ([a-z]+) is re-referenced after the \/ .

### Look-ahead and Look-behind

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/

Look-ahead (?=) and Look-behind (?<=) are not used in our example but essentially they allow us to set a search to either check a pattern that is followed by a specific character or check a pattern that is preceded by a speciific character.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
