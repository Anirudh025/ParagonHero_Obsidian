---
tags:
  - obsidian
---
#obsidian 
[Obsidian Help](https://help.obsidian.md)
# Basic formatting

### Paragraphs

This is a paragraph.

This is another paragraph.

### Headings
```
# # {heading title} 1
## ## {heading title} 2
### ### {heading title} 3
#### #### {heading title} 4
##### ##### {heading title} 5
###### ###### {heading title} 6
```

### Styled text
**BOLD** uses ** or __ around text
*ITALIC* uses * or _ around text
~~Strikethrough~~ uses ~~ around text
==Highlight== uses == around text <!--SR:!2023-08-31,4,270-->

### Quotes

> You can add a quote by using > before text
> \-[Obsidian](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax)

>[!info] You can turn your quote into a "callout" by using !info in aquare brackets

#### Other call outs
>[!tip]- !tip gives title
>and content

>[!faq]- using "-" makes it foldable
>Makes this go away

>[!todo] finish work

>[!success]- !success
>there's this

>[!question]- There can be a !question
>and an answer

>[!warning]- !warning
>Warns

>[!failure]- !failure
>fails

>[!danger]- !danger
>Another way to warn really

>[!bug]- !bug
>bugs

>[!example]- gives an !example
>use - after square brackets

![Hacker| 150x100](markus-spiske-666905-unsplash.jpg) Image is there

### List
You can create an unordered list by adding a `-`, `*`, or `+` before the text.

##### Unordered list
- list item 1
+ list item 2
* list item 3

##### Ordered list
1. list item 1
2. list item 2
3. list item 3

##### Nested list
1. List item 1
	1. Sub 1
+ List item 1
	+ Sub 1

##### Task list
- [ ] task 1
	- [ ] sub task 1
	- [ ] sub task 2 
- [ ] task 2
- [ ] task 3

### Separators

###### Use any of these:
```
***
****
* * *
---
----
- - -
___
____
_ _ _
```

##### To make a separator like this:
***

>[!info]- Another use of these separators
>to make a dropdown section

### Comments
use %% %% to make comments[^3]
```
%% comment %%
```
>[!info] Comments are only visible in editing mode

### Footnotes
 
 simple footnote[^1].
 
 make a foot note by adding ^{number} in square brackets. 

You can also use inline footnotes. [^This is an inline footnote]

[^1]: This is the referenced text.
[^2]: Add 2 spaces at the start of each new line.
  This lets you write footnotes that span multiple lines.
[^note]: Named footnotes still appears as numbers, but can make it easier to identify and link references.
[^3]: This is a footnote.
  footnote part added by leaving 2 spaces
[^note]: another note


# Advanced Formatting

### Tables

``` md
First Column | Second Column
-- | --
t1 | t2
t3 | t4
```

| First Column | Second Column |
| ------------ | ------------- |
| t1           | t2            |
| t3           | t4            |

```md
Left-aligned text | Center-aligned text | Right-aligned text
:-- | :--: | --:
Content | Content | Content
```
### Iframes and Embeds 

use for webpages
```html
<iframe src="INSERT YOUR URL HERE"></iframe>
```
[aknfa](sdfdfdknfkdn)