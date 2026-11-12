---
title: "When Licenses Clash"
teaching: 20 # draft; the group has not yet written the teaching content for this time
exercises: 10
---

:::::: questions

- What is a dependency?
- How do I find the licenses of my dependencies?
- What happens if a dependency has a license that does not fit my project?

::::::

:::::: objectives

- Identify the dependencies of a project.
- Find the license of each dependency.
- Decide whether a dependency's license fits what you want to do with your project.
- Describe an example of a license clash.

::::::

::::::::::::::::::::::::::::::::::::: instructor

### Narrative outline: Valentina (draft for the group to edit)

- Valentina wants to share part of her project and keep part closed.
- She installed packages through a package manager and has never checked their licenses.
- Her question: do the licenses of her dependencies allow what she wants?
- Needs from the group: a worked clash example and the compatibility rules.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: instructor

### Notes for this episode (draft)

This episode is a skeleton. Sections marked `TODO (group)` in the source need text from the cohort or a licensing expert. The slides give two bullets on dependencies and nothing on clashes.

- Timing plan: about 20 minutes of teaching and 10 of exercises. The exercises below are drafts, and no one has timed them.
- Optional demonstration: show how to find a package license on the command line. In Python, run `pip show <package>`. In R, run `packageDescription("<package>")$License`. Output varies by package and version, so try the commands before class.
- Several points in this episode follow the discussion in [ABCs of Open Source Licensing](https://www.youtube.com/watch?v=MWA5fdV6wg8) (UC Open 2025). The lesson authors' notes are in `instructors/files/ucopen-2025-abcs-licensing-notes.md`. An expert should check each point.
- The CURIOSS "open source software disclosure form" pattern asks researchers for a list of third-party software and its licenses. It is a good model for the "list your dependencies" activity (CC BY 4.0, credit the CURIOSS organizers and contributors).

::::::::::::::::::::::::::::::::::::::::::::::::

## What is a dependency?

A dependency is a piece of software that your project needs in order to run or build. Examples are a package you install with `pip` or `install.packages()`, or a library your code calls.

Your toolchain, integrated development environment (IDE), or package manager may add dependencies for you. Those packages can bring their own dependencies. A compiler or toolchain can also insert code into your final program, so you may distribute code you never chose on purpose. Valentina installed a handful of packages, and each one has a license she has never read.

For example, a Python project can name only a few packages, such as `python`, `numpy`, and `pandas`. A lock file records the exact version of each one and every package they need in turn. In one UC workshop example, a project that names just `python` and `numpy` has a lock file with 47 more dependencies. You may need to check the license of each one.

This example is adapted from [Making Research Software Citable & Discoverable](https://zenodo.org/records/18615247) by Tim Dennis, Reid Otsuji, Leigh Phan, Karla Padilla, and Laura Langdon (UC Love Data Week, 2026), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Changes: shortened and reworded.

<!-- TODO (group): add direct versus transitive dependencies if the group wants the terms. -->

## Why can licenses clash?

When you use someone else's code, their license applies to what you do with it. Your project must follow the terms of every dependency license, and those terms can limit which license you may choose for your own code.

<!-- Draft for the expert to check. Assumes the dependency is combined with your code into one program that you distribute. -->

The table shows what usually happens when you combine your code with a dependency.

| Dependency license | What happens to the combined program | Example |
|---|---|---|
| Permissive | You can release the combined program under other terms, including closed terms. Keep the required notices. | BSD, MIT |
| Weak copyleft | The library keeps its own license. Your code can stay separate under its own license, for example when you link the library dynamically. | LGPL |
| Strong copyleft | The combined program must be released under the same license. | GPL |

Table: What happens when you combine your code with a dependency

Copyleft terms usually apply when you distribute the combined program, for example by giving it to someone outside your organization. A license can define distribution broadly. The GNU Affero General Public License (AGPL) also covers running the code on a network server, so some organizations restrict its use.

<!-- TODO (group, expert): worked clash example. Suggested story: Valentina's project is under a permissive license and she wants to keep one part closed. One dependency is under the GPL. What does the GPL ask of her? State the version, the linking, and the distribution. Also decide what counts as distribution inside a university. -->

## Find the licenses of your dependencies

Before you share a project, list its dependencies and record the license of each one.

Dependencies are not only code. Data can have a license too, and the license shown on a data record may not match the limits on the data behind it. In one example from a UC technology transfer office, datasets on Zenodo carried Creative Commons licenses, but the patient data they were built on had no commercial rights. Check where your data came from and what its source allows.

<!-- Draft from the UC Open 2026 COSS panel for the expert to check. -->

<!-- TODO (group): where to find a license (package page, `LICENSE` file, package metadata) and how to record it (a simple table: package, license, type). Link the CURIOSS disclosure form pattern if the group agrees. -->

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: list Valentina's dependencies

<!-- TODO (group): supply four or five real packages with their real licenses, including one weak copyleft and one strong copyleft package. -->

Valentina's project uses the packages in the table below. For each package, say which category its license belongs to: permissive, weak copyleft, or strong copyleft.

| Package | License |
|---|---|
| TODO | TODO |

Table: Valentina's packages and their licenses

::::::::::::::::::::::::::::::: solution

<!-- TODO (group): answer key for the table above. -->

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## Does the license fit?

<!-- TODO (group, expert): compatibility rules of thumb. Cover at least: permissive code in a project under any license, an LGPL library linked dynamically, GPL 2.0 and GPL 3.0 code in a larger project, and Apache 2.0 with GPL 2.0. State the version and the situation (modifying, linking, distributing) for each rule. -->

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: LGPL or GPL?

Valentina wants to keep part of her project closed.

1. A package under the LGPL is linked dynamically to her closed code. Must her own code also be under the LGPL?
2. A package under GPL 2.0 becomes part of the code she wants to share. What does that mean for her code?

::::::::::::::::::::::::::::::: solution

<!-- Draft answers from the Episode 2 text. An expert should confirm. -->

1. Not necessarily. A weak copyleft license such as the LGPL may allow dynamic linking without triggering the copyleft provision. Her code can stay under the license of her choice.
2. GPL 2.0 is strong copyleft, so her code would need to be placed under the terms of the GPL.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## How UC rates the licenses of code you use

The University of California publishes a chart that rates open source licenses for using and redistributing open source code at UC.
The color for each license is intended to give "merely a high level assessment of the relative risk that use of a particular OSS license will violate UC Policies".
The chart does not compare licenses with each other.
All open source licensing of Regents-owned copyrights requires approval of the appropriate delegated authority (usually your campus technology transfer office), regardless of the risk category.

The chart sorts licenses into low, moderate, and high risk for two situations: using code inside UC, and distributing it outside UC. In short:

- Low risk in every situation: BSD, MIT, Apache 1.x (not 2.0 or later), GPL 1.x and 2.x, LGPL 2.x (not 3.0 or "any later version"), and the Educational Community License 2.0.
- Moderate risk in some cases of distributing outside UC: Apache 2.0 and the Eclipse Public License when you distribute modified code, and MPL 2.0 when you distribute modified code or code that only calls its functions.
- High risk for distributing outside UC: GPL 3.0 and LGPL 3.0 in every case, and GNU Affero General Public License (AGPL) 3.0 in every case except code that only calls its functions, which is moderate.
- Inside UC, the patent-granting licenses (Apache 2.0, Eclipse, MPL 2.0, AGPL 3.0, GPL 3.0, LGPL 3.0) are low risk if you add the required Internal Use Notice (the Companion Guide describes it).

For any other open source license, contact the licensing office.

The full chart has every combination. Consult the University of California Office of the President [OSS Chart](https://security.ucop.edu/files/documents/resources/oss-chart.pdf) (17 April, 2018 version) and [OSS Chart Companion](https://security.ucop.edu/files/documents/resources/oss-chart-companion.pdf) (26 March, 2018).

::::::: challenge

## Challenge: mark the conflicts

<!-- TODO (group, expert): fix the assumptions. State the license versions, what "Commercial" means (proprietary terms), and whether the scenario involves modifying, linking, or distributing. Add an answer key and a way to say "it depends". -->

Each row gives the license of the dependency. Each column gives the license of **My project**.

Mark an X in each cell where there is a conflict. Leave the cell empty if there is no conflict.

| Dependency license | BSD | MIT | Apache | LGPL | GPL | Commercial |
|---|---|---|---|---|---|---|
| **BSD** | | | | | | |
| **GPL** | | | | | | |
| **Commercial** | | | | | | |

Table: Compatibility grid. Rows are dependency licenses. Columns are project licenses.

::::::::::::::::::::::::::::::: solution

<!-- TODO (group, expert): answer key for the grid. -->

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

:::::: keypoints

<!-- Draft from the episode text for the group to edit. -->

- A dependency is software that your project needs in order to run or build.
- Check the license of every dependency before you share your project.
- A dependency's license can limit the license you may choose for your own code.
- Copyleft terms usually apply when you distribute the combined program. The AGPL also covers network use.
- At UC, the risk chart and your campus technology transfer office guide what is allowed.

::::::
