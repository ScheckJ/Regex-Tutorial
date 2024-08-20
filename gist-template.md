# Regex Tutorial

Regular expressions (regex) are powerful tools for matching patterns in strings. This tutorial breaks down a regex used to match a valid email address.

Link to the public gist https://gist.github.com/ScheckJ/d66e580c1c6a6284848769d559ffcacc


## Summary

This regex makes sure an email address is properly formatted usinig the following: a local part, an @ symbol, a domain name, and a domain extension. The pattern is:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Anchors ensure that the regex pattern matches the entire string from start to finish.

'^' asserts the start, and $ asserts the end of the string.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present for a match.

'+' matches one or more characters.

{2,6} specifies that the domain extension is between 2 and 6 characters long.

### Grouping Constructs
Grouping Constructs allow us to treat multiple characters as a single unit.

() groups parts of the regex: local part, domain, and extension.

### Bracket Expressions
Bracket Expressions (also known as character classes) define a set of characters to match.

[a-z0-9_\.-] matches lowercase letters, digits, underscores, dots, and hyphens.
[\da-z\.-] allows digits, letters, dots, and hyphens in the domain.

### Character Classes
Character Classes provide a shorthand to match specific types of characters.

\d matches any digit.

### The OR Operator
The OR Operator (|) allows for matching one of several possible patterns.


### Flags
Flags modify the behavior of the regex, such as making it case-insensitive.


### Character Escapes
Character Escapes (\) are used to treat a normally special character as a literal character.

## Author

My name is Scheck Jah and I am a student at U of R's coding bootcamp. Contact me on Github at http://github.com/ScheckJ