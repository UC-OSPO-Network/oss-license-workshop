---
title: "Permissive vs Copyleft Licenses"
teaching: 15
exercises: 15
---

:::::::::::::::::::::::::::::::::::::: questions

- Put questions here

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- State what an OSS license must allow users to do
- State what a permissive license allows and requires, and give an example of a permissive license
- State what a copyleft license allows and requires, and give an example of a copyleft license
- State what a weak copyleft license allows and requires, and give an example of a soft copyleft license

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

This is a lesson created via The Carpentries Workbench. It is written in
[Pandoc-flavored Markdown](https://pandoc.org/MANUAL.html) for static files and
[R Markdown][r-markdown] for dynamic files that can render code into output. 
Please refer to the [Introduction to The Carpentries 
Workbench](https://carpentries.github.io/sandpaper-docs/) for full documentation.

What you need to know is that there are three sections required for a valid
Carpentries lesson:

 1. `questions` are displayed at the beginning of the episode to prime the
    learner for the content.
 2. `objectives` are the learning objectives for an episode displayed with
    the questions.
 3. `keypoints` are displayed at the end of the episode to reinforce the
    objectives.

:::::: prereq

### Buoyant Barnacle

The exercises in this episode correspond to the Buoyant Barnacle repository you
created in [the Introduction](introduction.md)

:::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Inline instructor notes can help inform instructors of timing challenges
associated with the lessons. They appear in the "Instructor View"

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

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
