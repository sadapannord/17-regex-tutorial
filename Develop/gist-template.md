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

A quantifier indicates the number of characters or expressions to match. In this expression we are using the + and {} quantifiers. The + is searching for the [characters](#character-classes) in the first and second groupings, while the {} is searching for between 2 and 6 characters in the third grouping.

### Character Classes

This expression contains 3 groupings of character classes. In the first grouping we are searching for the letters "a" through "z", the numbers 0 through 9, and the characters (\_.-). The second grouping is searching for numbers 0 through 9, letters "a" through "z", and the characters (.-). The third grouping is searching for letters "a" through "z". 

### Grouping and Capturing


### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
