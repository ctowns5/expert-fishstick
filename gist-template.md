# Explanation of a regex expression that can be used to detect if a string is a HEX code.

This gist will explain the components of a regex expression that can detect if a string is a HEX code.

## Summary

This regex can be used to detect if a string is a HEX code

# /#?([\da-fA-F]{2})([\da-fA-F]{2})([\da-fA-F]{2})/g

It works with or without the leading # and on uppercase or lowercase examples

## Table of Contents


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

### Quantifiers
? Match between 0 and 1 of the preceding token

{2} Match 2 of the preceding token

Matches the specified quantity of the previous token. {1,3} will match 1 to 3. {3} will match exactly 3. {3,} will match 3 or more.

### Character Classes

[] Character set, Match any character in the set

### Flags

g is indicating a global search which retains the index of the last match, allowing iterative searches.

### Grouping and Capturing
() capturing group, groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.

### Greedy and Lazy Match

\d Digit, matches any digit character (0-9)

a-f Range, matches a character in the range a to f (char code 97-102). Case sensitive.

A-F Range, matches a character in the range A to F (char code 65-70). Case sensitive.

### Boundaries

/ open, indicates the start of a regular exprexssion. The / at the end is close, everything after the close / is a flag. In this case the g is indicating a global search which retains the index of the last match, allowing iterative searches.

### references 
https://regexr.com/ was used as a reference for this gist.
## Author
### The Author is an aspiring software developer with many years of experience in the conferencing industry.
### Link to GitHub profile: https://github.com/ctowns5

