# Dr. Regex: How I Learned to Stop Worrying and Love Regular Expressions

A Regex (regular expression) is a sequence of characters that define a search pattern. Generally, these patterns are used by algorithms that use a string-searching method for "find" or "find and replace" operations on strings, as well as searching for input validation.

## Summary

In this tutorial, we will be explaining the components of a regular expression, and how it works to create patterns for matching text. We will cover anchors, quantifiers, grouping contructs, bracket expressions, character classes, OR operator, flags, and character escapes.

We will be examining a Regex dealing with matching an email. Here is an example of a string that would do that- `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` and below we will discuss the components.

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

Anchors are used to specify the position of a pattern within the text being matched. The two most common anchors used in regular expressions are `^` (the Caret symbol) and `$` (the Dollar sign). The Caret symbol is used to match the beginning of a line, and the Dollar sign is used to match the end of a line.

You can also use `\b` which matches a word boundary position between a word character and a non-word character or position (start/ end of string) or you can use `\B` which will match any position that is not a word boundary - it only matches positions, not a character.

### Quantifiers

Quantifies specify how many time a preceding element should occur in the text being matched. There are many quantifiers that you can use:

- `*` The asterisk is used to match zero or more occurrences of the preceding element
- `+` The plus sign is used to match one of more occurrences of the preceding element
- `?` The question mark is used to match zero or one occurrences of the preceding element
- `{n}` Curly braces are used to specify an exact number of the occurrences of the preceding element
- `{n,}` Curly braces with a comma are used to specify a minumum number of occurrences of a preceding element
- `{n,m}` Curly braces with a comma between two values is used to specify a range of occurrences of a preceding element

### Grouping Constructs

- Capturing group `()` - Groups together elements and also captures and remembers matched text for later use, referenced or retrieved using backreferences
- Non Capturing group `(?: )` - Similar to capturing groups as in they group together elements, but they do not capture or remember the matched text. Useful when needing to apply operations to a group of elements but do not need to reference them later.
- Lookahead and Lookbehind assertions allow you to assert if certain characters or patterns are present of not present ahead of or behind the current position without consuming characters in the match. The symbols here are listed below:
  - Lookahead Positive `(?= )`
  - Lookahead Negative `(?! )`
  - Lookbehind Positive `(?<= )`
  - Lookbehind Negative `(?<! )`

### Bracket Expressions

In this example `([a-z0-9_\.-]+)` is a bracket expression that matches one or more lower case letters, digits, underscores, dots or hyphens in the username part of an email address.

### Character Classes

- `@` Matches the "@" symbol, and `\.` matches a dot character

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
