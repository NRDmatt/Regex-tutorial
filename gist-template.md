# Regex tutorial

Today I will be explaining certain components of a random regex code snippet with a brief description and a code snippet as example 

## Summary
I will be dissecting this snippet of regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$

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
Anchors: Anchors are special characters that match the position of the text, rather than the text itself. The section on anchors likely covers regular expression syntax for matching the beginning or end of a string, or other specific positions within a string.

^ - Matches the start of the string.
$ - Matches the end of the string.

### Quantifiers

Quantifiers: Quantifiers are special characters that modify the behavior of other regular expression syntax. The section on quantifiers likely covers syntax for matching one or more occurrences of a character, matching zero or one occurrences, or matching a specific number of occurrences.

"+" - Matches one or more occurrences of the preceding character or group. It is used in the character classes [a-z0-9_\.-], [\da-z\.-] and [a-z\.].
{2,6} 
\
"-" Matches the preceding character or group between 2 and 6 times. It is used in the character class [a-z\.] to match the top-level domain of the email address.

### OR Operator
OR Operator: The OR operator is a special character that allows you to specify multiple options for a regular expression match. The section on the OR operator likely covers syntax for specifying multiple alternatives in a regular expression.\

This snippet does not have any OR operators.

### Character Classes
Character Classes: Character classes are sets of characters that match a single character from a given set of possibilities. The section on character classes likely covers syntax for matching specific types of characters, such as digits, letters, whitespace, or punctuation.

"\d" - Matches any digit character (equivalent to [0-9]). \
a-z - Matches any lowercase letter from a to z.\
"0-9" - Matches any digit from 0 to 9.

### Flags
Flags: Flags are special characters that modify the behavior of regular expression syntax. The section on flags likely covers syntax for specifying case-insensitive matches, global matches, or other special behaviors.



### Grouping and Capturing
Grouping and Capturing: Grouping and capturing allow you to specify parts of a regular expression match that should be saved for later use. The section on grouping and capturing likely covers syntax for creating capturing groups, and accessing their values in later regular expression matches.

([a-z0-9_\.-]+) - matches and captures one or more lowercase letters, digits, underscores, dots, or hyphens before the "@" symbol.\
([\da-z\.-]+) - matches and captures one or more digits, lowercase letters, dots, or hyphens after the "@" symbol and before the "." in the domain name.\
([a-z\.]{2,6}|org) - matches and captures the top-level domain name which can be either a sequence of two to six lowercase letters or the string "org".

### Bracket Expressions
Bracket Expressions: Bracket expressions are another way to specify character classes in regular expressions. The section on bracket expressions likely covers syntax for matching ranges of characters, matching character sets, or matching special characters.

[a-z0-9_\.-] - matches any character that is a lowercase letter, a digit, an underscore, a period, or a hyphen.\
[\da-z\.-] - matches any character that is a digit, a lowercase letter, a period, or a hyphen.\
[a-z\.]{2,6} - matches any sequence of 2 to 6 characters that are lowercase letters or periods.

### Greedy and Lazy Match
Greedy and Lazy Match: Greedy and lazy matching are two different ways that regular expressions can match strings. The section on greedy and lazy matching likely covers syntax for matching the longest or shortest possible substring that satisfies a regular expression.\

 All matches are greedy by default. This means that the regex engine will match as much as possible while still allowing the entire pattern to match.


### Boundaries
Boundaries: Boundaries are special characters that match the beginning or end of a word, or other specific positions within a word. The section on boundaries likely covers syntax for matching the beginning or end of a word, or for matching specific positions within a word.\

'^' and $ are used as boundary matchers.

### Back-references
Back-references: Back-references allow you to reuse capturing groups from earlier matches in a regular expression. The section on back-references likely covers syntax for referencing earlier capturing groups in a regular expression.

### Look-ahead and Look-behind
Look-ahead and Look-behind: Look-ahead and look-behind are special syntax for specifying matches that are followed or preceded by specific characters or strings. The section on look-ahead and look-behind likely covers syntax for matching characters based on what comes before or after them in a string.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
