# Email Regex

Regular expressions, often called regex, are like supercharged search patterns that make it easy to find and manipulate text in a flexible way. They're handy in programming, text editors, and even when working with data. With regex, you can set up rules to find specific words, patterns, or conditions within text, making tasks like checking if an email is valid, finding and replacing words in a document, or extracting information from a messy dataset much easier. It's a powerful tool that's commonly used by developers, tech folks, and anyone who deals with text and data in their college projects or coding adventures.

## Summary

The regex we will be going over today will be one that matches/validates email addreses. Below is the regex of that does this. This is just one way of doing this. There are endless ways of making this regex.

Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

If we break this down this is what this regex is looking for.

([a-z0-9_\.-]+) Match one or more lowercase letters, numbers, underscores, dots, or hyphens for the username part
@([\da-z\.-]+) Match one or more digits, lowercase letters, dots, or hyphens for the domain name part
([a-z\.]{2,6})$ Match a period followed by two to six lowercase letters or dots for the top-level domain (TLD)

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

These are the various parts that help build the rules around the regular expression.

### Anchors

^ symbolizes the start of the string. $ symbolizes the end of the string.

### Quantifiers

- means that the preceding value/element should occur one or more times. For example, [a-z0-9_\.-]+ means we're looking for one or more lowercase letters, numbers, underscores, dots, or hyphes.

### Grouping Constructs

() means that we are grouping these values/elements together. So all the 'rules' or quantifiers within the parantheses would only apply to that group.

### Bracket Expressions

[a-z0-9_\.-]: This matches any single character that is a lowercase letter, a digit, an underscore, a dot, or a hyphen.
[\da-z\.-]: Matches any single character that is a digit, a lowercase letter, a dot, or a hyphen.
[a-z\.]: Matches any single character that is a lowercase letter or a dot.

### Character Classes

\d represents any digits [0-9]

### The OR Operator

There is no OR operator here

### Flags

There are no flags here

### Character Escapes

\.: This escapes the dot character, treating it as a literal dot instead of its special regex meaning (matching any character).

## Author

Paul Jang - a willing noob to coding. https://github.com/pjang77
