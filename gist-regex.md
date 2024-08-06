# Matching an Email – Regex Tutorial

What is A regular expression(regex for short)? It is a sequence of characters that defines a search pattern. This is commonly used to find patterns within a string, validate input or find and replace characters within a string. This tutortial will  walk you through the components of a regex and how it applies to matching an email.


## Summary

In this tutorial I am going to explain the use of regex and how to match emails using the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 

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
A regex is considered a literal, so the pattern must be wrapped in slash characters (/). If we examine the “Matching an Email” regex, you'll see that this is true:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This series of characters might not make sense to us, but it’s actually a search pattern meant for basic email validation. That is, it will checks to see if a string fulfills all requirements for a basic username. In a clamshell, here’s how it breaks down :

-The string can contain any lowercase letter between a–z

-The string can contain any number between 0–9

-The string can contain an underscore or hyphen

-The string is between 3–16 characters long


### Anchors

### Quantifiers

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
