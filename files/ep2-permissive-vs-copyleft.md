---
title: "Permissive vs Copyleft Licenses (DRAFT from slides)"
teaching: 15
exercises: 0
---

<!-- Source: 2026-OSPO-licensing-presentation.pdf, slides 10 to 14. Text follows the slides. Wording fixes are limited to typos. -->
<!-- TODO (group): questions and keypoints are left for the cohort to write. -->

:::::::::::::::::::::::::::::::::::::: questions

- TODO (group)

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

<!-- Objectives below are from the Day 1 lesson design notes, not from the slides. -->

- Identify the difference between permissive and non-permissive (copyleft) licenses, with an example of each
- List the most common open source licenses

::::::::::::::::::::::::::::::::::::::::::::::::

## Open source licenses

An open source license:

- is royalty-free, meaning end users do not pay any money
- permits the licensee (the end user) to use, copy, modify, and distribute the software
- comes with source code made available to end users, so they can exercise those rights

## License categories

Open source licenses fall into a spectrum. Permissive licenses sit on one side and strong copyleft licenses on the other.

<!-- The slides have no figure for this spectrum. A diagram could go here. -->

## Permissive licenses

Examples: BSD, MIT, Apache 2.0.

Permissive licenses have few requirements and are relatively easy to comply with. Typically, you are required to provide attribution. These licenses are common in research because they are simple and maximize flexibility. <!-- [KP1] comment marker from the source slide: a reviewer note, author unknown. -->

These licenses allow users to distribute your software commercially if they choose to.

At the University of California, BSD and MIT are favored over the Apache license. The Apache license requires licensors to grant a patent license to all licensees. This could have the unintended effect of reaching into UC's patent portfolio and the work of other researchers. With patents, different people or groups can come up with the same idea independently.

## Copyleft licenses

At the other end of the spectrum are copyleft licenses. They are sometimes called viral licenses, because they require that derivative works and modifications be licensed under the same terms as the copyleft license. This protects the openness of a project across its lifecycle.

Copyleft licenses may define what counts as a derivative work and what triggers the copyleft provision. So there are weak and strong copyleft licenses.

A weak copyleft license typically limits either the scope of what counts as a derivative work, or the trigger. For example, the LGPL may allow you to dynamically link to an LGPL library without triggering the copyleft provision. Your code that links to the library can then stay under the license of your choice.

## GPL 2.0 and 3.0

GPL 2.0 is a strong copyleft license. It would require your code to be placed under the terms of the GPL.

The UC system does not recommend GPL 3.0 for university-owned software, because its patent provisions may conflict with UC policies. If you need copyleft protection, consult your campus Tech Transfer office about GPL 2.0 or alternatives.

::::::::::::::::::::::::::::::::::::: keypoints

- TODO (group)

::::::::::::::::::::::::::::::::::::::::::::::::
