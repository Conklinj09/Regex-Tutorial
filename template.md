# Regex Tutorial
Matching an Email

Regex is it's own type of language with it's own library, a mini programming language. 
It uses regular expressions to process data and algorithms into different functions. The function we will be learning today is Matching an Email. 

## Summary

Matching an email. 
Here is the regular expression used:  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.
Each character inside this sentence has it's own function. 
We will be going over the functions inside each character of this expression. 


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
You can use regular expression components to match URL parameters or page names when configuring content for groups, custom reports, and URL rebuilding definitions. Regular expressions are a more useful tool because it provides more flexibility and powerful pattern matching that can be achieved. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors
Usually only at the end or at the beginning of a line, they are the first characters in an expression that usually consist of a caret (^) and the ($) dollar sign. The caret is found in the beginning, and the dollar sign towards the end. So if an expression starts with ^B it will match lines that start with uppercase B. If an expression ends with $B, it means the expression will match with all lines that end with uppercase B.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Quantifiers
Quantifiers specify how many times a character, group, or character class must be present in the input in order for a match to be found. 
Greedy quantifier     Lazy quantifier
*                          *?         matches zero or more times. 
+                          +?         matches one or more times. 
?                          ??         Matches zero or one time.
{ n }                      { n }?     Matches exactly n times. 
{ n , }                    { n , }?   Matches at least n times.
{ n , m }                  { n , m }? Matches from n to m times. 
The quantities n and m are integer constants. Quantifiers are greedy. They cause the regular expression engine to match as few occurences as possible. Appending the ? character to a quantifier makes it lazy. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/



### Grouping Constructs
When you place round brackets or parenthesis around the regular expression. You can do this to parts of it as well to group certain functions together, or to apply quantifiers to only a part of the group. It can also create numbered capturing group. It stores part of the string matched by the part of the regular expression inside the parentheses. 
Non-capturing groups are for when you don't need the group to catch it's match. 
Here is the expression for the non-capturing function to be initialized: Set(?:Value)?
Using text matched by Capturing Groups. Capturing Groups make it easy to extract part of the regex match. You can use the text inside the regular expression with a backreference. 
Backreference can also be used in replacement strings.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/



### Bracket Expressions
Bracket expressions are a list of characters and/or classes enclosed in brackets []. Use bracket expressions to match single characters in a list, or a range of characters in a list. 
If the first character of the list is the caret (^) then it matches characters that are not in the list. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/



### Character Classes
Here are the following character classes:
\d- digits
\D- non-digits.
\s- space symbols,tabs,newlines.
\s-S- all but \s.
\w- Latin letters, digits, underscore''.
\W- all but \w.
.- any character if with tthe regexp 's' flag, otherwise any except a newline \n.
With a character class, also known as the character set, you can tell the regex 
engine to match only one out of several characters. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### The OR Operator
In simple natural language, the alternation of the word OR is used to express multiple choices. 
For example knowing a language of English, French, or Spanish. 
But specified as a Condition in regex, this means that the operator(Logical OR) is used to match characters from one side to the other. For example, (gG) Will match either G or g from input string. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Flags
There are exactly 6 flags in javascript regex:

i    With this flag the search is case-insensitive: no difference between A and a 
g    With this flag the search looks for all matches, without it – only the first match is returned.
m    Multiline mode
s    Enables “dotall” mode, that allows a dot . to match newline character \n
u    Enables full Unicode support. The flag enables correct processing of surrogate pairs. 
y    “Sticky” mode: searching at the exact position in the text 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Character Escapes
The backslash character ( \ ) is the escaping character. It can be used to denote an escaped character, a string, literal, or one of the set of supported special characters. Use a double backslash ( \\ ) to denote an escaped string literal. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Author

Jeanette Conklin

https://github.com/Conklinj09/Regex-Tutorial


