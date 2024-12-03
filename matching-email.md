# Title (replace with your title)

Regex: Matching an Email

## Summary

Regex is a sequesnce of characters that creates a search pattern. It is used to match strings of text in a body of text, which can validate input, find patterns in strings, or find/replace characters in a string. This guide will show how to use Regex to match an email.

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

The string appears this way: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

We will break these components down. The `/` at the beginning and end of the string contains the string. 

### Anchors

The `^` anchors the regex at the beginning of the string. This means that a string will follow it. The `$`, also an anchor, means that the string ends. Everything between these characters determine what characters can be valid in an email. 

### Quantifiers

Quantifiers determine how many times an element can repeat. The `+` quantifier means that the characters inside the square brackets must appear one or more times. 

### OR Operator

Regex email does not contain an OR operator!

### Character Classes

Character classes define a set of characters that can be matched. These are frequently housed in square brackets `[]`. In this expression, `\d` is an example of a character class. There are many different character classes, but `\d` means the string can match any numeral between 0-9. 

### Flags

No flags are used in the email Regex!

### Grouping and Capturing

There are set constructs for how an email is to be formatted. To validate this formatting, grouping is used. Grouping is done with parenthases `()`. There are three groups in the email matching string, which seperates the email string into before the local part (before the @ symbol), after the domain part (after the @ symbol), and the TLD (after the dot). 

### Bracket Expressions

The bracket expressions such as `[a-z]` are used to define sets/ranges of chatacters. `[a-z]` specifically matches any lowercase letter. 

### Greedy and Lazy Match

In Regex, the default is for the program to be greedy, which means it will attempt to match as much text as possible. A lazy match tries to match the smallest amount of text possible. The quanatifier `+` is greedy, because it matches as many of the defined characters or strings as possible. There are no lazy matches in this text, but an example would be adding a `?` after a qualifier. For example, `+?` would be lazy due to only matching the shortest string that starts and ends with specific characters or strings. 

### Boundaries

There are no boundaries used in this text!

### Back-references

There are no back references used in this text!

### Look-ahead and Look-behind

There are no look-ahead or look-behined assertions in this text!

## Author

This tutorial was written by Noah McKinzie. Noah is a full stack developer working on graduating from the University of Texas at Austin Web Development Bootcamp! Please reach out with questions to me at nmckinzie@smcm.edu. You can find more of my work at <https://github.com/nmck-sys>.