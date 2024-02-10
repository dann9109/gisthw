# Regex tutorial

Regular expressions, often referred to as regex, are powerful tools used in programming and search algorithms to search for specific patterns in text. They consist of a sequence of characters that define the pattern to be matched. Regular expressions can be used to search for specific strings or patterns of characters within a larger text, and they can also be used to replace or manipulate text based on certain criteria. Additionally, regular expressions are commonly used for validating user input, ensuring that it matches the desired pattern or format.

## Summary

In this tutorial we are going to look at a common email regex sequence. This sequence can be used to validate legitimate emails in inputs and databases. Here is our example:

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

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
In regex, anchors are used to denote the beginning and end of an assertion or the matching process to validate a set of characters. In our email regex ^ indicates the beginning of a string, while a $ indicates the end of that same string.
### Quantifiers
Quantifiers specify the number of times a specific element or group should occur. In our email regex example, the + quantifier is used to indicate that the preceding group [a-z0-9_.-] should appear one or more times. This ensures that there is at least one alphanumeric or special character before the @ symbol.
### Grouping Constructs
Grouping constructs are used to group multiple elements together. They are enclosed in parentheses ( ). In our email regex example, the groups ([a-z0-9_.-]+), ([\da-z.-]+), and ([a-z.]{2,6}) are used to group specific parts of the email address, such as the username, domain, and top-level domain (TLD).
### Bracket Expressions
Bracket expressions, also known as character classes, specify a set of characters that can match a single character at a specific position. In our email regex example, the bracket expression [a-z0-9_.-] matches any lowercase letter, digit, underscore, dot, or hyphen. It ensures that the characters within the bracket expression are valid for the email address.
### Character Classes
Character classes represent a set of characters that can match a single character. They are defined within square brackets [ ]. In our email regex example, the character class [\da-z] matches any digit or lowercase letter.
### The OR Operator
The OR operator, denoted by the | symbol, allows for multiple alternatives to be specified. In our email regex example, the expression (.com|.org|.edu) matches either .com, .org, or .edu as a top-level domain (TLD).
### Flags
Flags are optional parameters that can be added to the end of a regex pattern to modify its behavior. In our email regex example, the / character at the beginning and end of the regex pattern serves as a delimiter, while the g flag indicates a global search for all matches.
### Character Escapes
Character escapes allow special characters to be matched literally instead of their inherent regex meaning. In our email regex example, the . escapes the dot character . to match a literal dot rather than any character. This is necessary when specifying the dot as part of the TLD.
## Author

(https://github.com/dann9109) I'm a student working on my journey to becoming a fulltime MERN fullstack developer