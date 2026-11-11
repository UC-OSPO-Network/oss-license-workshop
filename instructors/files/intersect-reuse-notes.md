# Reuse notes: INTERSECT "Software Licensing" lesson

Source: https://intersect-training.org/software-licensing/ (repository: INTERSECT-training/software-licensing).
License: CC BY 4.0, per the README badge and the page footer.
Authors listed in the README: David E. Bernholdt, Lauren E. Milechin, Dave Rumph, Michael A. Heroux, James Willenbring.

CC BY 4.0 needs credit (title, authors, source, license) and a note of changes. The source's own `CITATION.cff` and citation page still say FIXME, and the repository's `LICENSE.md` is the Carpentries template text. Credit the README authors, and check with the INTERSECT maintainers if a formal citation matters.

## Used

* "Is this an open source license?" exercise (episode "What is Open Source?"), in `episodes/permissive-vs-copyleft.md`. Credit and changes are stated under the exercise.

## Not used, and why

* The "Popular OSI-approved licenses" table (episode "Choosing an Open Source License").
  * It labels MPL 2.0 and CDDL 1.0 "permissive". Our Episode 2 keypoints call MPL weak copyleft.
  * It says "any license on this list is a good choice". UC guidance in our slides favors BSD and MIT over Apache and does not recommend GPL 3.0 for university-owned software.
  * It marks EPL 2.0 as GPL-compatible with no condition. Check that against FSF guidance before using it.
  * Decision for the cohort: build our own comparison from UC sources, or adapt this table with UC caveats.
* Their definition of "derivative work" quotes Wikipedia (CC BY-SA). Do not copy that sentence.

## Possible later use

* Choosing and documenting a license (file headers, badges): extends slides 19 and 20.
* Contributor agreements, code copied from forums, and LLM-generated code: candidate future episodes.
* The OSI-approved definition: fills a TBD glossary entry (#26). Check the exact wording at the source before copying.
