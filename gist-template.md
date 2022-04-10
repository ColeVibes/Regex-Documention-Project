# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

In this Gist I will be explaining the details of the regular expression used to validate an email. Shown in regex format the expression is ``` /^[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/ ```. With this documentation I hope to show you the full scope of the regex and help others use it to the fullest extent.

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

This regex can be broken down in varous components, in this instance that is ```[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]``` detailing the possible expressions before the @ symbol is placed, ```+@``` detailing the need for an @ symbol and ```[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]``` stating the possible expressions that can take place after the @ symbol happens.

### Anchors
Anchors are a family of regex tokens such as ```^``` or ```$``` that pertain to the string or the matching process inside the expression of characters. In the email validation regex there are several to designate. 

- The ```^``` symbol is used as a starting anchor in the expression.
- The ```$``` symbol is used to end the string in which the system will check.

### Quantifiers
Quantifiers are symbols that are used to specify how many times a regular expression must match to the characters following the quantifier symbols. In this expression there we are currently only using one.

- The "```+```" symbol is used to match one or more of the characters the proceed it.

An example in this expression is ```+@```, which breaks down into the direct need to match one or more characters of the ```@``` symbol in the email address. To learn more about the other tokens availiable to use as a quantifiers read this article (https://www.fon.hum.uva.nl/praat/manual/Regular_expressions_2__Quantifiers.html)

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
