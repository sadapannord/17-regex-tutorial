# How to verify if text is an Email

This article is an explanation of the regular expression (also known as regex) commonly used to determine if a string contains an email. This article contains a detailed explanation of each component of the regex.

## Summary

The article details each component of the /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ regex, which when implemented determines if text contains all the elements that an email is comprised of.

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

### Anchors

This regex contains "anchors" which search the beginning and end of string. The ^ character searches the beginning, and the $ searches for the end. In our regex, the beginning anchor is searching for a [grouping](#grouping-capturing) of characters preceding the @ symbol, and the ending anchor is searching for a grouping that follow a period (.).

### Quantifiers

A quantifier indicates the number of characters or expressions to match.

### OR Operator

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
