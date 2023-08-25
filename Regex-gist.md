<p align="center">
  <img src="./imgs/recipeforregexsmall.png" />
</p>

<p align="center">
<h1 align="center">INTRODUCTION</h1>
REGEXs at first glance look super infurtiating and diffuclt! Thought that may be the case (lol) it is something that we will be traversing throughout this tutorial to try and explain the functionality and how helpful REGEX can be when using them! 
</p>

<p align="center">
  <img src="./imgs/schoolofrock.gif" />
</p>


## Summary of what a REGEX is!

Think of having your own codex for a large group of jumbled letters and words that make no sense! Imagine having a code breaker that can notice patterns in the huge jumbled mess. THAT is similarly how a REGEX works when implemented in your code! 

More specifically in definition, a REGEX is a felxible set/sequence of characters that interprets whatever defined pattern is associated to the expression. A REGEX can come in handy considering it's primarily used for pattern matching within strings of text. With REGEX you can manipulate, identify, or search for specific portions of text based on a set of rules you define!

For example, REGEX patterns can be used for a myriad of operations, a couple being but not limited to:
- Matching Social Security Numbers
- Validation
- Text search and Manipulation
- Data Extraction
- Language Processing

Coming up in the next section we will begin breaking down an example of  a REGEX and how it functions!

The REGEX that we will be breaking down is MATCHING A URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`
<p align="center">
  <img src="./imgs/magnifying glass.gif" />
</p>

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## REGEX Components

### Anchors
Anchors are special characters in a REGEX that don't match any actual characters. Instead, they state positions inside the input text. The two main anchors are:
- ^ (caret): Matches the start of a line or string.
- $ (dollar sign): Matches the end of a line or string.

### Quantifiers
Quantifiers define how many times a specific element should appear in the input for a match to be triggered. There is a great bit of flexibility added REGEX patterns. Common quantifiers include:
- *: Matches zero or more occurrences.
- +: Matches one or more occurrences.
- ?: Matches zero or one occurrence.
- {n}: Matches exactly n occurrences.
- {n,}: Matches at least n occurrences.
- {n,m}: Matches between n and m occurrences.

### Grouping Constructs
Grouping constructs gives you the opportinity to group characters together. Utilizing grouping constructs can be useful for associating quantifiers to many characters, capturing portions of the match, or applying alternation. They are enclosed within parentheses `( )`.

### Bracket Expressions
Bracket expressions give you the ability to specify a set of characters that the REGEX engine will match to a single character. They are surrounded by square brackets [ ].

### Character Classes
Character classes, commonly known as predefined character classes, are short notations that explain common sets of characters.
- \d: Matches any digit.
- \w: Matches any word character (alphanumeric + underscore).
- \s: Matches any whitespace character.
- \D, \W, \S: Negations of \d, \w, and \s, respectively.

### The OR Operator
The OR operator, also commonly known as "The other character on the backslash key" (just a little joke) , allows you to specify other patterns. It matches either the pattern on the left or the pattern on the right. It's used for creating choices in your REGEX.

### Flags
Flags are optional settings that you can apply to your REGEX to change its behavior.
- i: Case-insensitive matching.
- g: Global matching (find all occurrences).
- m: Multi-line matching.

### Character Escapes
Character escapes allow you to match characters that would more generally have special meanings in REGEX. For example, \. matches a literal dot (period), and \\ matches a literal backslash.

## REGEX BREAKDOWN
`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

So what we will do is now go and explain component by component what the above REGEX can be used for! 

1. `/`: Forward slash at the start of the REGEX clarifies the start of the regular expression.
2. `^`: The caret indicates the start of the line or string, which tells us that the match should start from the beginning.
3. `(https?:\/\/)?`: This optional group matches the protocol part of a URL. It can match "http://" or "https://". The s? makes the 's' optional, and \/\/ matches the two slashes after the protocol.
4. `([\da-z\.-]+)`: This gets the domain name part of the URL. It includes digits, lowercase letters, dots, and hyphens. This usually is for the subdomain or domain name.
5. `\.([a-z\.]{2,6})`: This gets the top-level domain (TLD) part of the URL, like ".com" etc. It matches a dot followed by 2 to 6 lowercase letters or dots. This range covers more common TLD lengths.
6. `([\/\w \.-]*)*`: This gets the path part of the URL. This particular instance allows for multiple segments in the path, each separated by a slash. The segments can have a variation of word characters, spaces, dots, and hyphens.
7. `\/?$`: This specifies an optional slash at the end of the URL. The \/ matches a slash, and the $ defines the end of the line or string.
8. `$`: This indicates the end of the line or string, also clarifying to the REGEX that the match should continue until the end.
9. `/`: The last Forward slash at the end of the REGEX tells us that this is now the end of the REGEX, similar to how strings use `"`


## Author

My name is Ismael Jimenez-Jurado, my family and friends call me `Nano`! I am currently a Software QA Engineer at Eduphoria! Inc. and am also at the end of a Full-stack Web Developer Bootcamp at the University of Arizona! (Go Wildcats!!!)

If you have any questions about the tutorial or just want to connect and collaborate, please feel free to reach out and contact me at any of the specified links below!

<p align="center">
  <img src="./imgs/rollcredits.gif" />
</p>

# CONTACT ME!
[![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/ismael-jimenez-jurado/)
&nbsp;
[![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/Idjjurado)
&nbsp;
[💌💌💌Email me](mailto:ismael.david.jimenez@gmail.com)
