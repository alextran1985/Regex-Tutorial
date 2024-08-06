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

/^([a-z0-9_\.-]+) @([\da-z\.-]+)\.([a-z\. ]{2,6})$/

This series of characters might not make sense to us, but it’s actually a search pattern meant for basic email validation. That is, it will checks to see if a string fulfills all requirements for a basic email. It can be broken down in three parts :

First part : ([a-z0-9_\.-]+) matches the user email name.

-The string can contain any lowercase letter between a–z
-The string can contain any number between 0–9
-The string can contain an underscores (_), periods (.), and    hyphens (-).
-The (+)  represent one or more of the characters in the preceding character class.

Second part: @([\da-z\.-]+)\ matches the domain name.

-(@): Matches the literal @ character.
-(/d): Matches the digits 0-9.
-The string can contain any lowercase letter between a–z
-The string can contain an periods (.) and  hyphens (-).
-The (+)  represent one or more of the characters in the preceding character class.

Third part: .([a-z\. ]{2,6}) matches the top-level-domain(TLD).

-The string can contain any lowercase letter between a–z
-The string can contain an periods (.)
-The length must be between 2 and 6 characters.

### Anchors
The symbol ^ and $ are both considered to be anchors. The ^ anchor signifies the beginning of a sting. And the $ anchor signifies ends of the stings.

### Quantifiers

Quantifliers set the limits of the string that your regex matches and usually appeared before the ($) anchor ({2,6}).

### OR Operator

OR Operator add same logic outside of a bracket expression within a grouping construct and is usually represented by the (|). [abc]=(a|b|c).

### Character Classes

Character Classes defines a set of characters which can occur in an input string to fulfill a match. Here are some examples:

-(.)—Matches any character except the newline character (\n)

-(\d)—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

-(\w)—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). This class is equivalent to the bracket expression [A-Za-z0-9_].

-(\s)—Matches a single whitespace character, including tabs and line breaks

### Flags

Flags are placed at the end of a regex usually after the second slash and define additional functionailty or limits. Here are some examples:

-(g)—Global search:  should be tested against all possible matches in a string.

-(i)—Case-insensitive search: case should be ignored while attempting a match in a string.

-(m)—Multi-line search: a multi-line input string should be treated as multiple lines.

### Grouping and Capturing

Grouping constructs break sections up to determine that different sections fulfill diffent requirements. And do by using parentheses(()).

### Bracket Expressions

Bracket Expressions are anything inside the set of square barckets([]) represents the range of characters we want to match. They are also know as positive character group, because they outline all the characters we want to use.

### Greedy and Lazy Match
Greedy is when Quantifiers can match as many occurrences of a particular patterns as possible. Example are:

-(*)—can match the pattern zero or more times

-(+)—can match the pattern one or more times

-(?)—can match the pattern zero or one time

Lazy Match can be made by adding the (?) and will match as few occurrences as possible.

## Author

GitHub profile: https://github.com/alextran1985
