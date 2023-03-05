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

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

Hello! I am Cesar, and I am a student currently enrolled in UT's fullstack coding bootcamp. I'm coming into this field from a customer service background, wanting to learn something new that is different from what I am used to. We can connect via my github: 