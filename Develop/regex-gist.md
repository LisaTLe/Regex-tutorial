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

### Character Classes

Character classes are usually represented with square brackets `[]`. Letters and numbers can be placed inside the brackets to state certain requirements. For example, `[A-Z]` means that characters can range anywhere from A to Z but they will be case-sensitive. It will be the same when teh bracket looks like this, `[a-z]`. When `[\d]` is used, this will be a representation for digits (0-9). This is also equivalent to `[0-9]`.

### Flags

Flags can be used to modify searches in regular expressions. The flags will change how the string search will be interpreted. Here are a list of common flags used:

- i : This will cause the search to be case-insensitive which means that there will be no difference between A and a.
- g : This stands for global search. This will look for all matches.
- m : This flag stands for multiline mode. This will find matches on multiple lines.
- s : This flag is known as a dotall. It will match any character along with newline characters.
- u : This enables full unicode support. Which means that the flag enables correct processing of surrogate pairs. It is used for extended unicode.
- y : this is known as sticky mode. This will allow for searching at the exact position in the text.

### Grouping and Capturing

Groups are represented by `()` and can contain multiple expressions. Groups are used in an expression to narrow down password parameters. When there are multiple expressions in a group, it is considered a capture group.

### Bracket Expressions

Bracket expressions are characters that are placed inside of `[]`. It will be able to match a single character in the list inside of the bracket.

### Greedy and Lazy Match

Lazy match means to repeat minimal number of times. Which means that it will match to a few characters as possible. For greedy match, it is the opposite of lazy match. The quantified character will be repeated as many times as possible.

### Boundaries

Boundaries are shown in two ways:

- \b : is also recognized as an anchor. It matches at a position called a word boundary. It is a zero-length match. This allows tou ro perform "whole words only" search.

- \B : this will match at every and any position between two word characters. It can also be at any position between two non-word characters as well. This is known as a not word boundary.

### Back-references

Back-references match the same text as previouslt matched by a capturing group. These are also known as numeric references.

### Look-ahead and Look-behind

Look-ahead and look-behind are collectively called "look-around". These are zero-length assertions that match characters but then gives up the match. This will only return the result, match or no match.

## Author

My name is Lisa Le and I am a full stack developer student. You can find more of my work at https://github.com/LisaTLe.
