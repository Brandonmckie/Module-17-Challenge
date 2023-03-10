# Match an Email - Regex Tutorial

This tutorial is going to explain the use of regex to match emails using the expression /^/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

## Summary

A regular expression is a pattern of characters that is used to search for specific patterns within a string. It is frequently utilized to find and replace characters within a string, as well as to validate input. This tutorial will explore the various components of a regular expression and demonstrate how they are employed to match an email address.

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

Regular expressions are made up of different parts that can help you create search patterns. Some common parts include Character Classes, Groups, Quantifiers, Anchors, Lookarounds, and more.

When you put these parts together, regular expressions can be hard to understand but they can also help you find exactly what you're looking for. With the right parts, you can find almost any combination of words or letters.

### Anchors

In regular expressions, the characters ^ and $ are both considered to be anchors. The anchor ^ indicates that the following character should be the begining of the string, and the $ proceds the ending of a string.

### Quantifiers

This regular expression uses the + operator as a quantifier to concatenate the user's email name, email service, and .com. It also employs the {2,6} quantifier to match a range of 2-6 characters from the character set of [a-z.].

### Grouping Constructs

The regular expression's character class \d matches a single digit from 0-9. Therefore, it will match a single character such as "4", but not multiple digits like "44".

### Bracket Expressions

Expressions enclosed in brackets used for email validation encompass the following character sets: [a-z0-9_\.-], which matches any case-sensitive letter from a to z, any character from 0 to 9, and the characters "\_", "-", and ".". Additionally, [\da-z\.-] matches a single digit from 0 to 9, any case-sensitive character from a to z, and the characters "." and "-". Lastly, [a-z\.] matches any case-sensitive character from a to z and the character ".".

### Character Classes

The regular expression's character class, \d, matches a single digit character from 0-9. This means that it will only match a single digit, like "4", but not multiple digits such as "44".

### The OR Operator

The expression [abc] can be rewritten using the OR operator (|) as (a|b|c). For example, if we have a string that can contain any of the characters a, b, or c, we can use the regular expression (a|b|c) to match any occurrence of these characters in the string.

### Flags

Optional flags can be added to a regular expression by placing them at the end of the regex after the second slash. These flags provide additional functionality or limitations to the regex. There are six available flags that can be used independently or combined in any order.

### Character Escapes

In regular expressions, the backslash (\) is used to escape a character that would otherwise be interpreted literally. This means that if a special character needs to be searched for, it can be escaped with a backslash to look for that specific character.

For instance, the open curly brace ({) is typically used to begin a quantifier in a regular expression. However, by adding a backslash before the open curly brace (\{), the regular expression will search for the literal open curly brace character instead of treating it as the start of a quantifier. This is a common practice when searching for strings that contain special characters that are identical to a specific component of a regular expression.

## Author

This was written by Brandon Mckie you can find my projects at https://github.com/Brandonmckie
