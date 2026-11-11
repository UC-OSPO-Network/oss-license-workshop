# Persona-based challenge ideas and Episode 4 questions (draft for the group)

Bare bones. These are ideas for authors to build on, not finished exercises. Every expected answer needs a licensing expert to check it. The design notes ask for multiple choice questions where the wrong answers are real misconceptions ("no license means public domain", "permissive means anything goes", "copyleft is viral").

The Carpentries Handbook says to carry a narrative through examples and exercises, so learners can recognize the concept in repeated chances.

## Episode 1: Camila

* Use the existing "accidental trap" case study as Camila's project. No new exercise.
* Quick poll: Camila's collaborator says "it is on GitHub, so it is public domain." True or false? Targets the misconception in the Myth or Fact opener. Source: slide 6.

## Episode 2: Camila

* Multiple choice: Camila wants anyone, including companies, to reuse her code with few conditions. Which license type fits? Correct: permissive (BSD, MIT). Source: slide 12.
* Multiple choice: Camila wants improvements to her code shared back. Correct: copyleft. Source: slide 13.
* Wrong answers to include:
  * "A permissive license means attribution is not needed." Slide 12 says attribution is typically required.
  * "Copyleft means companies cannot use the code." Copyleft allows any use. Check against the Episode 2 keypoints.
  * "UC prefers Apache 2.0." Slide 12 says UC favors BSD and MIT, because of the Apache patent grant.
* The XYZZY exercise stays as it is. It does not use a persona.

## Episode 3: Valentina

* Activity: Valentina lists the packages her project uses, with each package's license and type. The group supplies the package list. The CURIOSS pattern "open source software disclosure form" asks researchers for exactly this list of third-party software and licenses (CC BY 4.0, credit the CURIOSS organizers and contributors).
* Multiple choice, slide-supported: a package under the LGPL is linked dynamically. Must Valentina's own code also be LGPL? Slide 13: the LGPL may allow dynamic linking without triggering the copyleft provision.
* Multiple choice, slide-supported: a package under GPL 2.0 is part of the code she wants to share. What does that mean for her code? Slide 14: GPL 2.0 would require her code to be under the GPL.
* Gap: compatibility rules and the answer key for the existing grid. The group must supply these.

## Episode 4: Santiago (capstone)

1. Who typically owns the tool Santiago wrote as part of his staff job? Correct: The Regents of the University of California. Wrong answers: Santiago ("I wrote it"), the campus group, the collaborator. Source: slide 8.
2. Who approves releasing it as open source? Correct: the Tech Transfer office, as the campus delegated authority, whatever the license's risk rating. Wrong answer: Santiago, once he picks a license from the UC list. Source: slides 9 and 16, and the UC chart legend.
3. Which license should Santiago choose from the UC-recommended list? Correct for this scenario: a low-risk license such as BSD 3-Clause. Wrong answers: GPL 3.0 (UC does not recommend it for university-owned software), Apache 2.0 (UC favors BSD and MIT). Source: slides 12 and 14.
4. Hands-on: add the BSD 3-Clause LICENSE file with the Regents as copyright holder, then add the License section to the README. This is the challenge already in Episode 4 (slides 18 to 20).

## Proposed "questions" block for Episode 4

The current block holds three exercise plans, not learner questions. Suggested questions, taken from the slide content:

* Who owns software I wrote at UC, and who approves releasing it?
* How do I choose a license from the UC-recommended list?
* How do I show which license my project uses?

The three exercise plans in the block (think-pair-share, matching, multiple choice) could move into the episode as exercises. That is Karla's content, so the group decides (#9).

## Not drafted

Keypoints for all four episodes. The group writes those.
