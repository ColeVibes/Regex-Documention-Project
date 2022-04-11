# Email Validation Regex Expression

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
In some coding languages symbols like the "|" symbol which can be used to search for one set of characters OR another set, in this example there are no "or" operators. Another common operator is the Range Operator as shown below.

- A great example in this expression is ```[a-zA-Z0-9-]```. With this you can see three different "-" symbols, telling the search to look for any character in-between ```a-z```, ```A-Z```, and ```0-9```. In this instance we can find either upper, or lower-case letters because we have specified that either are okay to be present. 

For more information on other common operators you can visit (https://support.workiva.com/hc/en-us/articles/4407304269204-Regular-expression-operators)

### Character Classes
Character Classes are any symbols enclosed in a set of ```square brackets```. In this instanc there are two sets of character classes that the expression looks for.

-While both are searching for basically the same things, the character classes are ```[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]``` and ```[a-zA-Z0-9-]``` with the second instance being repeated twice. 
- In this we can see that the search is looking for various symbols, the letter "a-z" and all letter in-between, special characters such as "." or "!" are also included. Each character class is enclosed with "[]" brackets to start and end.

### Flags
Flags are single, lowercase letters that have the search continue in a different way. One such example is a lower-case "m", which lets the system search for thing by goping through multiple lines of code at once. In this instance of email validation, there are none used.

### Grouping and Capturing
Both and capturing set characters together to be searched for in sequence, and they are set in "()" with the characters being grouped or captured in the middle.

- This regex has one complete group that is classified as a non-captured group in the expression. The set ```(?:\.[a-zA-Z0-9-]+)``` uses the "()" symbols, along with the "?" and ":" symbols to set a non-captured group that creates a single unit of all the symbols in the middle.

### Bracket Expressions
Brackets are used to create a matching, or non-matching list. In this instance the lists we have are ranged expressions and character classes. Each set by either the "[]" brackets or "()" in the instance of the group present.

### Greedy and Lazy Match
Both Greedy and Lazy matching search for the same thing, it is just that both expressions look for the same search parameters in different ways. 
- Greedy matching is the default way for searchs to occur, with it the search extracts as much as possible from the expression to fit the desired pattern, even if the pattern could be matched with less data. 
- Lazy matching is a simpler way to match a given pattern, it takes a symbole such as ```?``` after a quantifier to search for that symbol the least amount of times possible.

### Boundaries
A boundry used in regex is a symbol such as ```-``` used at the beginning or end of a string or number to seek matches. 

- In the example "-12" the ```-``` symbol searches for a match of either the number 1, or 2.

### Back-references
Back-references are used in regular expressions to find an already match word or pattern to another one later in the string or number.

### Look-ahead and Look-behind
A look-ahead and a look-nehind are the same search parameter just in reverse. A look-ahead sets a parameter to look for s symbol or string ahead of the parameter, and a look-behind does the opposite.

## Author
You can find me at [GitHub](https://github.com/ColeVibes) for more info or projects.
