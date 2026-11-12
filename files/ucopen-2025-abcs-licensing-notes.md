# Notes: "ABCs of Open Source Licensing" (UC Open 2025)

Source: "UC Open 2025 ABCs of Open Source Licensing", a directed discussion led by Karla Padilla (UCSD) and Jeff Shapiro (Linux Foundation). UC Open 2025. The session took place on 24 April 2025 (see https://ucospo.net/events/uc-open-4-2025/sessions/licensing/). The video was uploaded on 30 May 2025 and runs 51 minutes. Video: https://www.youtube.com/watch?v=MWA5fdV6wg8 (UC Open Source Program Office, UC Santa Cruz channel).

These are the lesson authors' own notes with approximate timestamps. They are not a transcript. The video has no stated reuse license, so the lesson links to it and does not copy it. The talk is the likely origin of slide 15 (toolchains and dependencies).

The speaker's statements are practitioner views, not legal advice. An expert should check each point before it becomes lesson text.

## Points and where they could go

| Time | Point | Lesson use |
|---|---|---|
| 2:06 to 4:30 | An open source license grants the rights to copy, modify, and redistribute. Common obligations: attribution, contributing changes back (some licenses), same-license release of derivative works (copyleft), and a warranty disclaimer. | Episode 1 and Episode 2 (already covered). |
| 6:05 to 8:30 | Two classes: permissive and copyleft. Copyleft is divided into strong and weak. Permissive licenses mix more easily with commercial or proprietary code. | Episode 2 (already covered). |
| 8:37 to 9:50 | Public domain is not a license. Seeing source code does not make software open source. | Episode 1 or the glossary. |
| 10:33 to 11:00 | At UC, BSD and MIT are preferred. Apache is not preferred because of its patent clauses. | Episode 2 (already covered). |
| 11:26 to 14:40 | LGPL gives an exception for dynamic linking. The GPL with Classpath Exception exists because Java does not link the same way. | Episode 2 weak copyleft and Episode 3 (LGPL challenge). |
| 15:31 to 17:30 | Copyright is not a license. Copyright exists when you write code. If you cannot find a license, do not assume the code is open source. | Episode 1 (already covered). |
| 17:43 to 19:30 | Contributor license agreements (CLA) and the developer certificate of origin (DCO). | Possible later episode. |
| 19:44 to 25:40 | SPDX license identifiers. A comment that says only "BSD" is ambiguous, because there are many BSD licenses (0, 2, 3, and 4 clause). Use the exact identifier. | Episode 2 (same family) and Episode 4 (communicate your license). |
| 20:42 to 22:00 | Most large applications are 70 to 90 percent open source code. A software bill of materials (SBOM) lists the pieces. | Episode 3 (dependencies). |
| 25:52 to 28:06 | Mixing table. Permissive code with proprietary code: the combined work can be proprietary. Weak copyleft: the library keeps its license, and your code can stay separate. Strong copyleft: the combined work must use the same license. | Episode 3 (compatibility rules). |
| 31:01 to 32:20 | Choose a well-known license so people and their legal teams recognize it. | Episode 4 (how to choose). |
| 33:17 to 33:50 | Funders may require OSI-approved licenses. | Episode 4 (ownership and funders). |
| 36:12 to 41:40 | Copyleft is typically triggered by distribution. A license can define distribution broadly. The AGPL counts network use, so many organizations avoid it. A tech transfer story: a sticky library surfaced late in due diligence. | Episode 3 (copyleft trigger). |
| 42:28 to 43:30 | OSI publishes the Open Source Definition and a list of approved licenses. A license can be open source without being on that list. | Glossary entry for "OSI-approved". |
| 43:38 to 45:30 | A license that bars commercial use is "source available", not open source. The UC Academic License is the example. | Episode 2 callout on non-commercial use. |
| 45:36 to 47:00 | Toolchains and package managers can insert code into your product. Know your dependencies. | Episode 3 (dependencies). |

## Open questions for an expert

* Is "many organizations avoid the AGPL" something the lesson should say?
* The talk calls the UC Academic License "source available". Confirm that before the lesson repeats it.
* What counts as distribution inside a university or a network?

## Also reviewed: UC Love Data Week 2026 deck

"Making Research Software Citable & Discoverable" (Dennis, Otsuji, Phan, Padilla, Langdon; 11 February 2026), CC BY 4.0, https://zenodo.org/records/18615247. A copy is in `instructors/files/2026-UCLDW-sharing-software.pdf`. Pages 10 to 17 repeat the licensing slides already mapped to the episodes. New material used, with credit in the episodes:

* "Idea" lines for permissive and copyleft licenses (page 12): Episode 2.
* The pixi example of a short dependency list and a lock file with 47 more dependencies (pages 20 to 22): Episode 3.
* "UC standard recommendation: BSD 3-Clause" (page 16): Episode 4, marked for expert review. A panelist at UC Open 2026 said UCLA may move to BSD 3-Clause Clear.
* The UC OSPO README template (page 38) and stating the license in `CITATION.cff` and on Zenodo (pages 34 to 40): Episode 4.

Not used yet: the FAIR4RS link (license is part of "Reusable", pages 6 to 9) could frame Episode 1.
