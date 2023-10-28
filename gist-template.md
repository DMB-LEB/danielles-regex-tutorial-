# danielles-regex-tutorial
As part of my coding bootcamp's weekly challenge we are to breakdown an email matching regex.

## Summary
A regex, or regular expression, is a case sensitive string of letters, numbers, or symbols used to search a longer string. 

An example of an email matching regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/  


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
There are two anchors, ^ and $. The ^ anchor is at the beginning of a string that signifies there are characters to follow, meanwhile $ is found at the end of a string that signifies characters that precede it.

### Quantifiers
Quantifiers dictate the quantity of characters that should be matched. The following quantifiers * and + try to match as many characters of the string as possible, while ? will stop as soon as it locates a match. Brackets with a postive number inside such as, {n}, allows you to search for a specific character of a string keeping in mind the quantity you are looking for. For example we were searching an email string for "l{2}," "Danielle" should pull up, but "Daniel" should not. Another type of quantifier that includes brackets look like {n,m}. You can picture this as m>n. The search should return the minimum, "n" to the maximum, "m".

### Grouping Constructs
Groups are constructed by parenthesis, anything within the parenthesis would be part of a group.

### Bracket Expressions
Bracket Expressions [] allow to match a specific set of characters, example [a-z] or [*, %, @].

### Character Classes
Charcter classes are a type of Bracket Expressions, as seen in my example above [a-z]. Another example would be [abcde].

### The OR Operator
The OR Operator looks like |. This may come in handy when searching for an email domain. Say you are just looking for "@google.com" or "@yahoo.com"

### Flags
Flags include i, g, m, s, u, y.
 - i: Makes search case-insesitive
 - g: Pulls up all matches
 - m: Stands for multiline mode
 - s: Enables "dotall" mode
 - u: Unicode mode
 - y: "Sticky" mode 

### Character Escapes
To use a special character as a regular character the special character you are looking to use must have a backslash, \, preceeding it.

## Author
Bootcamp student at UNH. To see more please visit my GitHub - https://github.com/DMB-LEB
