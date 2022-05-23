# Joel's Regex Tutorial

Wanting to learn about the wonderous world of regular expressions? You've come to the right place! Contained within this arcane codex, you will find the secrets to mastering the Magick of the regular expression (AKA Regex). Regexes are of massive utility, for they can pull information from any body of text by looking for one (or more) matches of a search pattern. You, as an aspiring Code Mage, can harness their power for data validation, web scraping, molding strings to your whim, etc. A beautiful aspect to learning regexes is that they can be utilized in virtually all programming languages!

## Summary

As an emample, let's break down the components of this ancient & mysterious regular expression, which matches an Email address:\
\
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/  
\
This document will unravel its clandestine nature, and allow you to cast the spell, for yourself, in your future coding adventures!

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

According to javascripttutorial.net:\
"Anchors have special meaning in regular expressions. They do not match any character. Instead, they match a position before or after characters".\
The anchors in our example dictate the beginning and the end of what is being matched; the ^ indicates the beginning of what's being matched, and the $ indicates the end of what's being matched.

### Quantifiers

The MDN definition of regex quantifiers is as follows:\
"Quantifiers indicate numbers of characters or expressions to match."\
In the example, we have 2 different types of quantifiers. We have two instances of the + quantifier, and one instance of {2,6}. The + says we are matching 1 or more of the preceding token. The {2,6} means we are matching between 2 and 6 of the preceding token.

<!-- ### OR Operator -->

### Character Classes

A character class, or character set, tells the regex to match only the characters listed within square brackets []. This can be a specific few characters, or a range of characters. In our example, you can see the following character classes:\
[a-z0-9_\.-]\
This one includes all letters a-z, all numbers 0-9, an underscore, a period (with a forward slash for escaping), or a dash \
\
[\da-z\.-]\
This one includes any digit character 0-9 (with "\d"), a character in the range a-z, a period, or a dash \
\
[a-z\.]\
This one includes all letters a-z, and a period \
\

<!-- ### Flags -->

### Grouping and Capturing

According to oracle.com, "Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. For example, the regular expression (dog) creates a single group containing the letters 'd' 'o' and 'g' ."
In our example, we have 3 groups for capture: ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}). This will allow the regex to match our search parameters in the three parts of an Email address; joel@gmail.com would match in our a groups as joel, gmail and com.

### Bracket Expressions

The bracket expressions are what's contained inside the square brackets []. In our example, they contain our character classes, or sets.

<!-- ### Greedy and Lazy Match -->

<!-- ### Boundaries -->

<!-- ### Back-references -->

<!-- ### Look-ahead and Look-behind -->

## Author

Joel Cutler is a particularly rad individual, and an accomplished mage. He dabbles in many forms of magic, including: caloriemancy (vegetable farming), soil necromancy (regenerative agriculture), cold-temperature downhill teleportation (snowboarding), elemental toolmaking (coding), and participates in paladin training to round out his melee game (Krav Maga).

His GitHub can be found here:\
[GitHub: joelcutler](https://github.com/joelcutler)
