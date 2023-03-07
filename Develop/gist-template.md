# How to verify if text is an Email

This article is an explanation of the regular expression (also known as regex) commonly used to determine if a string contains an email. This article contains a detailed explanation of each component of the regex.

## Summary

The article details each component of the /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ regex, which when implemented determines if text contains all the elements that an email is comprised of.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

### Anchors

This regex contains "anchors" which search the beginning and end of string. The ^ character searches the beginning, and the $ searches for the end. In our regex, the beginning anchor is searching for a [grouping](#grouping-capturing) of characters preceding the @ symbol, and the ending anchor is searching for a grouping that follows a period (.).

### Quantifiers

A quantifier indicates the number of characters or expressions to match. In this expression we are using the + and {} quantifiers. The \([a-z0-9_\.-]+) is searching for the [characters](#character-classes) in the first and second groupings, while the \{2,6} is searching for between 2 and 6 characters in the third grouping.

### Character Classes

This expression contains 3 groupings of character classes, enclosed in square brackets []. The first is \[a-z0-9\_\.-] the second is \[\da-z\.-] and the third is \[a-z\.]. We are also searching for any digit between 0 and 9 in the snipped [\da-z\.-] following the @ symbol.

### Grouping and Capturing

A grouping is a way to use multiple characters as a single object, this is created by placing the characters in parenthesis (). This expression contains 3 groupings. The first is preceding the @ symbol ([a-z0-9_\.-]+), the second directly afterwards ([\da-z\.-]+), and the third following a period ([a-z\.]{2,6}). A group that is "captured" contains all the characters that were matched.

### Bracket Expressions

Bracket expressions are used to determine what characters we are searching for. In the first grouping we are searching for the letters "a" through "z", the numbers 0 through 9, and the characters (\_.-), in the code snippet \[a-z0-9\_\.-]. The second grouping is searching for numbers 0 through 9, letters "a" through "z", and the characters (.-) in the code snippet \[\da-z\.-]. The third grouping is searching for letters "a" through "z" in \[a-z\.].

### Greedy and Lazy Match

This regex contains greedy operators, meaning they will expand the match as far as they can through the provided input, this is denoted through the {} and + operators.

## Author

If you would like to view my GitHub profile please visit https://github.com/sadapannord
