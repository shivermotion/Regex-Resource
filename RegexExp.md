# Regex Explainer

## What is a Regex?

A **regex**, which is short for **regular expression**, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

This Gist is a tutorial on how to translate and breakdown a chosen Regex. Each component and piece of a regex will be broken down into its individual parts in the table of contents below.

the example regex used is:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

a common regex used for matching email addresses.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

We use `and / and ^ together at the beginning as a string anchor. $ Matches at the end of the string the regex pattern is applied to.

### Quantifiers

Quantifiers indicate numbers of characters or expressions to match. The simplest quantifier is a number in curly braces: {n}.

A quantifier is appended to a character and specifies how many we need. It can also be a range denoted as {n,n} so in our snippet `([a-z\.]{2,6})$/` {2,6} is the range of number of characters its looking for.

### Grouping Constructs

Groups and ranges indicate groups and ranges of expression characters. For example, [xyz] [a-c]. In our email regex one example would be a-z0-9 in `/^([a-z0-9_\.-]+)`. They then can be filled with such examples as a-z0-9 which matches any ASCII letter a-z or digit 0-9.

### Bracket Expressions

In the following first snippet `/^([a-z0-9_\.-]+)` of the regex, we can connotate the start of a character class using []. A bracket expression is a list of characters enclosed by ‘[’ and ‘] .

### Character Classes

The character class is the most basic regex concept. It makes one small sequence of characters match a larger set of characters. \d is used in the example regex to signify the character class, specifically digit.

## Author

created by:

Jason Day

jason.day.blue@gmail.com

github: https://github.com/shivermotion
