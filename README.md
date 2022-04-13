# Regex Tutorial for Matching a Hex Value


The purpose of this tutorial is to breakdown a regex and provide examples for each component. 

## Summary
--------------------------------------------------

The regex that will be broken down in this tutorial is for matching a hex value.

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Contents
--------------------------------------------------

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
--------------------------------------------------

### Anchors
- The `^` character indicates the start of the string that will be returned.
- The `$` character indicates the end of the string that will be returned. 
    - For example, `^abc$` as part of a regex, will return exactly `abc`.
### Quantifiers
- The curly brackets containing a number `{1}` indicates to search for the preceding character(s) that many times.
    - For example, `[a-f0-9]{6}` indicates to search for one character between the letters a-f and the numbers 0-9 exactly six times.
- The `?` character indicates to match the character preceding it either 0 or 1 time(s). Essentially meaning that that character is optional.
    - For example `#?` as part of a regex will include the `#` character in the return search if it contains it, but will not prevent a search from being returned if it does not contain it.
### OR Operator
- The `|` character indicates to search for one of multiple options.
    - For example, `([a-f0-9]{6}|[a-f0-9]{3})` will return matches of `[a-f0-9]` with six characters OR with three characters.
### Character Classes
- The bracket characters `[]` indicate to search for one of the characters within them. 
- The dash character `-` is a range indicator to search between two given characters.
    - For example, `[a-f0-9]` indicates to search for one character between the letters a-f and the numbers 0-9.
### Flags
- None in this regex
### Grouping and Capturing
- The parenthesis character `()` captures and remembers the charaters matched between the `()`.
    - For example, if the regex `([a-f0-9])` finds the character `a`, it will be read exactly as `a`.
### Bracket Expressions
- None in this regex

### Greedy and Lazy Match
- None in this regex

### Boundaries
- None in this regex

### Back-references
- None in this regex

### Look-ahead and Look-behind
- None in this regex

## Author

Lauren Rodenbusch-Yoder. Coder and cat mom extraordinaire. <br>
[GitHub](https://github.com/lrodenyoder)
