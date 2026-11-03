---
title: "Permissive vs Copyleft Licenses"
teaching: 15
exercises: 15
---

:::::::::::::::::::::::::::::::::::::: questions

- What must every open source license allow, no matter which one you pick?
- What does a permissive license ask of people who use your code, and what does a copyleft license ask instead?
- If two licenses are in the same family, does it matter which one you choose?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- State what an OSS license must allow users to do
- State what a permissive license allows and requires, and give an example of a permissive license
- State what a copyleft license allows and requires, and give an example of a copyleft license
- State what a weak copyleft license allows and requires, and give an example of a soft copyleft license

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

::::::::::::::::::::::::::::::::::::: callout

## "I want researchers to use this, but not companies"

This is one of the most common things researchers ask for, but it actually isn't compatible with the premise of open source. The [Open Source Definition](https://opensource.org/osd#:~:text=6.%20No%20Discrimination%20Against%20Fields%20of%20Endeavor) says a license "may not restrict the program from being used in a business."

If excluding commercial use really is a requirement, a license like [PolyForm Noncommercial](https://polyformproject.org/licenses/noncommercial/1.0.0) will do it. Researchers at academic institutions would still be able to use your code, but they couldn't build it into their own open source projects. Researchers at companies, startups, and industry labs couldn't use it at all.

::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 1: Can you do it?

What is the output of this command?

```r
paste("This", "new", "lesson", "looks", "good")
```

:::::::::::::::::::::::: solution 

## Output
 
```output
[1] "This new lesson looks good"
```

:::::::::::::::::::::::::::::::::


## Challenge 2: how do you nest solutions within challenge blocks?

:::::::::::::::::::::::: solution 

You can add a line with at least three colons and a `solution` tag.

:::::::::::::::::::::::::::::::::
::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints

- An open source license must let anyone use, study, change, and share the software, for any purpose, including commercial use
- Permissive licenses (MIT, BSD, Apache) let others reuse the code almost any way they like, including in closed-source products, as long as they keep the copyright and license notice
- Copyleft licenses (GPL) also allow any use, but anyone who distributes a modified version must share its source under the same license
- Weak copyleft licenses (LGPL, MPL) apply that rule only to the licensed code itself, so it can be combined with code under other licenses
- Licenses in the same family still differ on specific points, like patents and the use of contributors' names, so check the actual clauses before choosing
- Your institution's technology transfer office makes the final call

::::::::::::::::::::::::::::::::::::::::::::::::

[r-markdown]: https://rmarkdown.rstudio.com/
