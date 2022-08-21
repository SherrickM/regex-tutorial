# regex-tutorial

## Summary
---

In this tutorial, we will disscuss matching an e-mail using Regular-Expression a.k.a Regex. For reference, please take a look at the code snippet below. You will see the code snippet thoughout the remainder of this document.

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## GitHub Gist

> https://gist.github.com/SherrickM/269186a21458115644d422b0b712d27f
---
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
---
## Regex Components
---
### Anchors

1. Anchor Symbol ^
2. Anchor Symbol $

#### What are Anchors?
 
 - Anchors are regex tokens that don't match any characters but that say or assert(anchor) something about the string or the matching process. There are two ancors in regex; the caret(^)used to start the string and the dollar sign($) used to end the string. 

 Review the code snippet below to see if you can identiy the start ^ and the end $ of the string

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

---
### Quantifiers

#### What are Quantifiers?

- Quantifiers specify and measure how many characters must be present in the input field for a match to be found. In the code snippet below {2,6}, we are using a qualifer to state the input should be a minimum of 2 characters to a maximum of 6 characters

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
___
### Grouping Constructs

#### How to using Grouping Constructs? 

- By placing part of a regular expression inside round brackets () or parentheses, you can group that part of the regular expression together i.e. grouping constructs. 

  Looking at the code snippet below, there are three grouping consucts. 

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
1. ([a-z0-9_\.-]+)
2. ([\da-z\.-]+)
3. ([a-z\.]{2,6})

### Bracket Expressions

A bracket expression is anything found within square brackets []. It indicates a range of characters that tell us what we want to match within the text. In the code snippet below, there are three bracket expressions. 

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

1. [a-z], indicates any lower letters between a-z
2. [0-9], indicates any numbers between 0-9
3. [_\.-], indicates the special cartes that we can use.


---
### Character Classes

- Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits. The bracket expressions we discsuess in the previous section is an example.

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
---
### The OR Operator

- OR Operator symbol: |

- The "OR" operator "|" is to match the characters on the left or right of the operator. Using the OR Operator, a|A would match one of the two "s" or "S" from the string.

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
---
### Flags

- Flags are letters that come after the closing slash / that allow you to use some advanced features.  For example, "g"  indicates a global search, meaning your regex will match all possible patterns in a string instead of just return the first one it finds. While "i" indicates a search is non-case sensitive, or case-insensitive.

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
---

### Character Escapes

A character escape uses a backslash as the escape code, which restores the original literal meaning of the following character. 

> `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

---
## Author

Sherrick M

> https://github.com/SherrickM/regex-tutorial
