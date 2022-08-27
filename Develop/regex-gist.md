# RegEx Tutorial

RegEx is also known as "regular expression". It is a sequence of characters that defines a specific search pattern. RegEx can be used in code and algorithms to find specific patterns in a string, or it can also be used to find a replace a sequence in a string. In this tutorial, we will learn more about how RegEx is used by going over a specific regEx used for passwords. We will break down and define the specific search pattern used in the sequence.

## Summary

Passwords are important and are used in many online platforms. Learning more in depth about regex for password validation will be very useful for many developers. When creating a password, there are a set of requirements needed. Below is an expression used for validation of passwords.

regex = "^(?=._[0-9])(?=._[a-z])(?=._[A-Z])(?=._[@#$%^&-+=()])(?=\\S+$).{8, 20}$"

- Must contain a number
- Must have at least one lowercase and uppercase letter
- Must have at least one special character
- Must have a minumum of 8 characters but a maximum of 20 characters
- No spaces allowed

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

The anchors used in this string are `^` and `$`. To start off the string, `^` is used. To end the string `$` is used.

### Quantifiers

Quantifiers in regex expressions are `?`, `*`, `+`, `.`, and `{x,y}`. The `?` symbol represents that zero or one of a certain character or value is required. `*` symbol represents zero or more of a certian character or value is required. `+` means one or more of a certain character or value is required in the password. the `.` represents the match of any character other than linebreaks. `{x,y}` will give parameters as to what the minumum and maximum requirements for the string will be.

### OR Operator

The OR operator in regular expressions are pipe characters, `|`. This can be used to provide more than one term for an expression.
