# Regular Expression/ Regex Tutorial- Phone Number

This tutorial is for web developers to help them understand the search pattern the regex defines. This tutorial breaks down each part of the regular expression, or regex, and describes what it does.

## Summary

Regular expressions, or regex, are patterns used to match character combinations in strings. They allow users to search through text quickly. In this regex example users will validate a phone number.

The regular expression looks for:
 /^(?:\d{3}|\(\d{3}\))([-\/\.])\d{3}\1\d{4}$/
 
Users are promted to enter a phone number. When the user presses the "Check" button, the script checks the validity of the number. If the number is valid (matching the character sequence),  a message appears with confirmation of a valid number. If the number is invalid, a message informing the user to try agian using another the phone number.

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
/^(?:\d{3}|\(\d{3}\))([-\/\.])\d{3}\1\d{4}$/

### Anchors— ^ and $
The characters ^ and $ are both considered to be anchors, but do not match chatacters.
The ^ anchor signifies the beginning of a string and the The $ anchor signifies a string that ends with the characters that precede it.

### Quantifiers- * + ? and {}
Quantifiers specify the numbers of characters or expressions to match. It inculdes a minmum and maximum number of character the regex is looking for.

The ? indicates the expression to match 0 or 1 time. 
In the curly brackets the regex we have {3},{3},{3}, and {4}  this indicates that the length of these quantifiers. 
Example: #-###-###-####

### OR Operator— | or []
The "or" operator within a regular expression is defined using the | element. The or operator indicates that it could either of the components that we are separating with the | or []. The phone number regex has 4 components. 
/^(?:\d{3}|  
\(\d{3}\))
([-\/\.])  
\d{3}\1\d{4}$/

### Character Classes— \d \w \s and .
In this regular expression, the charactor class /d is used which in Javasctipt classifies the use of any digit from 0 to 9.


### Grouping and Capturing— ()
/^(?:\d{3}|\(\d{3}\))   captures the country code and area code 
([-\/\.])               captures numbers, periods, and hyphens



### Bracket Expressions — []

The information in the bracket expressions is opened and closed between brackets like this []. This indentifies which information is allowed to be matched.

Bracket Expression [-\/\.] - includes case sensitive characters, numbers , periods and hyphens.


### Greedy and Lazy Match ( * + {})
Expand the match as far as they can through the provided text.
{3}
{3}
{3}
{4}


### Back-references— \1
  \1 it matches the same text that was matched by the first capturing group 


## Author

My name is Staisha Knight and I'm a full-stack developer student looking to succeed and a grow in the tech industry. 

Github: https://github.com/StaishaKnight
