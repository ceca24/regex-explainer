# Understanding Regular Expression

Hello and welcome to a (Reg)ular (Ex)pression, or "Regex" for short, tutorial to know that a random text of characters actually have some meaning behind them. Regex is used in programming/computer science to define a search pattern in text form, or "string". By using this pattern, the Regex engine matches the pattern of the inputed string, or text, that consists of these "random" characters.

## Summary

Now, you may be thinking, "what are these random texts and characters is this person talking about?" Well, here is a nice example of one that will be broken down here:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

That seems a bit confusing, and a bit random, doesn't it? Well, allow me to give a brief summary of what is being "said" in this string. This regex defines the search pattern for a valid e-mail address. A good way to spot a regular expression is by the forward slashes (/) in the beginning and end of the text. Common examples of this format include "bighugger10@hotmail.com" or "iamtired@gmail.com". Let's dig into this regular expression, and learn the components that help make this regex a regex!

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

First things first, let's discuss the "Anchor" aspect of the regex. Anchors are special characters that that tell the reader where the string begins and where it ends. It begins with a carat (^) and ends with a dollar sign ($). These helps the reader to focus on a specific string, and makes the search more efficient since it is between the carat and dollar sign. Without these characters at the beginning and end of the string, the search engine will take longer to produce results since it will be looking for the pattern in other locations.

### Quantifiers

You may ask yourself, "What does 'Quantifiers' mean?" Well, the definition is "an expression that indicates the scope of a term to which it is attached". In regex, quantifiers will tell us how many times something is repeated, and is a part of the grouping. Though there are different types of quantifiers, in this example, curly brackets ({}) are the quantifiers. This can be used to make sure a value limit is exactly a certain amount of character. If left blank, the limit becomes infinite. With the above example {2, 6}, the quantifier is telling the reader that the item should be repeated at least two times, and up to 5 times. 

Other examples of quantifiers include a question mark (?), an asterisk (*), and the plus sign (+). Each of these carry their own range as shown below:

"?" = {0,1}
"*" = {0,}
"+" = {1,}

### Grouping Constructs

With Grouping Constructs, these are pretty straightforward. They can be found within parentheses "()", and work great when multiple bracket expressions are used. With the above example, there are three different grouping constructs, with their own paramaters set to allow certain types, or number of characters.

### Bracket Expressions

Bracket Expressions are used to define a set of characters that are allowed to be used in the regex within the square brackets "[]". In the above example, the first grouping construct is defined by the bracket expression "a-z0-9_\.-". This means that the first grouping construct can only contain lowercase letters, numbers, underscores, periods, and hyphens. The second grouping construct is defined by the bracket expression "a-z0-9\.-". This means that the second grouping construct can only contain lowercase letters, numbers, periods, and hyphens. The third grouping construct is defined by the bracket expression "a-z\." This means that the third grouping construct can only contain lowercase letters, periods, and hyphens.

### Character Classes

Character Classes help pick out the different kinds of characters the reader wants to check for, or match, in the regex and are indicated by a backslash "\". Including the above example, here are some of the most common character classes:
* \d = any digit
* \D = any non-digit
* \w = any word character
* \W = any non-word character
* \s = any whitespace character
* \S = any non-whitespace character

As the reader can see, the capital letter version of the character class will match the opposite of the lowercase version. For example, \d will match any digit, while \D will match any non-digit.

### The OR Operator

The OR Operator is used to match one of several possible pattern, being indicated by the pipe "|" symbol. For expression purposes, take this line for instance:

(here|there|everywhere)

This line will match the word "here", "there", OR "everywhere". This is a great way to match multiple words, or phrases, in a single line.

### Flags

Flags are used to modify the search pattern, and are indicated by a forward slash "/" at the end of the regex. The most common flags are "g", "i", and "m". The "g" flag is used to search for all matches in the string, while the "i" flag is used to ignore the case of the string. The "m" flag is used to search for multiple lines in the string.

### Character Escapes

Character Escapes are used to match special characters, and are indicated by a backslash "\". For example, if the reader wanted to match a period, they would use "\." instead of just ".". This is because the period is a special character, and would not be recognized by the regex engine without the backslash.

## Author

Hello! I am Cesar, and I am a student currently enrolled in UT's fullstack coding bootcamp. I'm coming into this field from a customer service background, wanting to learn something new that is different from what I am used to. We can connect via my [github](github.com/ceca24).
