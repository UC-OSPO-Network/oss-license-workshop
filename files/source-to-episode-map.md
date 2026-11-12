# Source to episode map (UC talks and decks)

Prepared 2026-11-12. This maps what each source offers to each episode and says what is likely to work well in teaching. The "effective" column is the lesson authors' judgment, not tested with learners.

All speaker statements are practitioner views, not legal advice. An expert checks each point before it becomes lesson text. None of the video text is copied. Links point to the videos.

## Sources read

| Source | Read | Link |
|---|---|---|
| UC Open 2025: ABCs of Open Source Licensing (Padilla, Shapiro) | 0:00 to 47:13 of 51:33 | https://www.youtube.com/watch?v=MWA5fdV6wg8 |
| UC Open 2025: Panel on Technology Transfer and Impact of Open Source (Padilla moderating; Oettinger, Kehle, MacDonald, Shayesteh) | 0:00 to 43:37 of 49:04 | https://www.youtube.com/watch?v=QZI1vicDTEo |
| UC Open 2025: Fireside chat on commercial open source (Meeker, Davis) | all | https://www.youtube.com/watch?v=Hsq0B5DH47s |
| UC Open 2026: Panel "Making a COSS Play" (Padilla chairing) | all (pasted by Tim) | https://www.youtube.com/watch?v=V4XjaDWG-cs |
| UC Love Data Week 2026 deck (CC BY 4.0) | pp. 1 to 46 | https://zenodo.org/records/18615247 |
| UC Open 2026: Breakout 1 "Open Practices for Education and Training" (includes the UC OSPO education talk) | keyword scan plus the AI and licenses exchange (about 1:04:00 and 1:16:42); the rest is about documentation tools such as MyST and Jupyter Book | https://www.youtube.com/watch?v=jqAcaQQR-Bs |
| UC Open 2025: Directed discussion "How can we help? Academic OSPOs" | keyword scan only; almost no licensing content | https://www.youtube.com/watch?v=5wUFC3mIz_g |
| UC Open 2025: "Open S#####? What is meant by open" | keyword scan only; about open science, almost no licensing | https://www.youtube.com/watch?v=q509nMUKan0 |
| UC Open 2025: Panel on supply chain security | keyword scan only; security focus, 19 mentions of dependencies | https://www.youtube.com/watch?v=LmTYcJD9s6o |

Not read: the 2026 keynotes and breakouts, the lightning talks, the agrifood, AI and vLLM sessions, and about 55 older videos on the channel (OSRE, workshops and others).

### Keyword scan of the other UC Open talks (2026-11-12)

| Talk | Licensing hits | Useful for the lesson |
|---|---|---|
| 2026 keynote, Nithya Ruff | 5 | Two points. Choosing community-governed projects lowers the risk that a license changes later. Models such as Llama and DeepSeek are "open weights", not open source, because their licenses carry restrictions. This could be an example in Episode 2 of a license that limits use. https://www.youtube.com/watch?v=1VtGcD4fQLY |
| 2026 keynote, David Charron | 1 | Nothing. Mostly commercialization history. https://www.youtube.com/watch?v=s1FHdA4ntPI |
| 2025 panel on open source in industry | 1 | Nothing. https://www.youtube.com/watch?v=_JepJmGtmf0 |
| 2025 panel "From Idea to Impact" | 4 | A first-hand story of how the BSD license began at UC Berkeley, and a UCSF project released under BSD. A possible narrative hook for Episode 2. https://www.youtube.com/watch?v=yVmVT-G92kM |

Still unscanned: the 2025 keynote on the impact of open source, the XZ security keynote, the ecosystems and innovation talk, the 2026 breakout 2 (1 hour 46 minutes), the 2026 opening and both sets of lightning talks, and the AI security, agrifood, and vLLM sessions, plus about 55 older videos. Titles suggest little licensing content.


## Karla's other records

* 23 April 2025: panel on technology transfer (she moderated). Read above.
* 24 April 2025: ABCs session. Read above.
* 11 February 2026: UC Love Data Week workshop. Read above.
* April 2026: COSS panel (chair).
* 8 to 23 September 2026 UC Carpentries workshop: she is listed as a helper, not an instructor. Day 23 September is "Sharing Research Software".
* 10 December 2026, Linux Foundation Open Compliance Summit (Tokyo): "Academic OSPOs on the Frontline of OSS Compliance in the University Setting". The abstract says licensing knowledge is uneven in academia and calls for outreach, training, and user-friendly SBOM tools. This describes our audience.

## Map by episode

### Episode 1: Why License?

| Point | Source | Recommendation | Effective? |
|---|---|---|---|
| License is the first piece of FAIR4RS "Reusable", with README, citation, and environment | Love Data Week deck, pp. 6 to 9, 42 | Open Episode 1 with a short framing: sharing code well needs a license, a README, and a citation. Licensing comes first. | Likely. It gives learners a reason before the myth and fact opener. Your call, because Episode 1 is Jose's content. |
| Common misconception: the person who writes the code owns it | Technology transfer panel (about 12:00) | Use as a think-pair-share or a "myth" statement. Currently the callout says software is "typically owned by The Regents". See the expert flag below. | High. The misconception is explicit and learners hold it. |
| If you cannot find a license, do not assume the code is open source | ABCs 17:03 | Already covered (think-pair-share). | Already works. |
| Copyright is not a license | ABCs 15:31 | Already covered. | |
| Public domain is not a license | ABCs 8:37 | Add one glossary entry. | Low effort. |

### Episode 2: Permissive vs Copyleft

| Point | Source | Recommendation | Effective? |
|---|---|---|---|
| Plain-language ideas for permissive and copyleft | Love Data Week deck | Used. | Likely. |
| BSD has many forms; a bare "BSD" is ambiguous | ABCs 24:00 | Used in the same-family section. | |
| BSD and MIT came from universities and have the fewest requirements | Tech transfer panel 27:48 | Add as one line in the UC-preference paragraph. | |
| Three buckets for a campus: closed or commercial, open source, academic non-commercial | Tech transfer panel 16:13 | Add a short callout after the "researchers but not companies" callout. Name the UCLA academic license and PolyForm as source available. | High. It answers "can I stop companies using it?" with options. |
| Source available is not open source | ABCs 43:38, panels | Used. | |
| Lawsuits over compliance exist (Vizio) | Tech transfer panel 28:30 | Optional instructor note. | Low. |

### Episode 3: When Licenses Clash

| Point | Source | Recommendation | Effective? |
|---|---|---|---|
| Mixing table: permissive, weak copyleft, strong copyleft | ABCs 25:52 | Used. Pair with Valentina's story. | High, as a table plus one worked example. |
| Copyleft triggers on distribution; AGPL covers network use | ABCs 36:12 | Used. | |
| Toolchains can insert code into your program | ABCs 45:36 | Used. | |
| Red in the UC chart does not mean forbidden. It needs the informed consent of the delegated authority, who may weigh the patent risk. | Tech transfer panel 42:23 | Add one sentence to the chart summary and one question to the Ep3 challenge. | High. It stops learners from reading the chart as a ban. |
| Why UC rates GPL 3.0 high risk: its patent grant covers every contributor, and the Regents hold copyright across all campuses | Tech transfer panel 24:50 | Add two sentences under the chart summary. Apache 2.0 was downgraded from red to yellow after review. | Medium. Explains the "why", which Elias wants. |
| Check the license of every dependency before you release; a license that conflicts with a dependency creates trouble | Fireside chat 33:08 | Reinforces the keypoint. | |
| Tech transfer officers review every library and its license during due diligence; for trained models they ask about data provenance | Tech transfer panel 29:05 | Use as the "why check" motivation for Valentina. | Medium. |
| A dataset can carry a Creative Commons license while the data underneath has no commercial rights | COSS panel 24:14 | Used. | |
| Dependencies as a supply chain security issue (SBOM, vulnerabilities) | Supply chain panel | Optional hook only. The panel is about security, not licensing. | Low for this lesson. |
| Pixi example: two named packages, 47 more in the lock file | Love Data Week deck p. 20 | Used. | High. Concrete and visual. |

### Episode 4: Choosing a License

| Point | Source | Recommendation | Effective? |
|---|---|---|---|
| Ownership first; sponsor and funder obligations come before the license | Tech transfer panel 16:37 | Add funders as the second ownership question. Already partly there. | High. |
| Delegated authority (usually the campus IP director) decides open, closed, hybrid, or no license; counsel only advises | Tech transfer panel 40:19 | Make this the answer to "who approves?". Add to the TTO section. | High. |
| If you contribute to an existing project, use that project's license; a red license needs informed consent | Tech transfer panel 41:30 | Add a short section or a fifth multiple-choice question. The original Ep4 objective mentions "contributing to different projects". | High. |
| Changing a license later is possible but painful | Fireside chat 13:20 | Add one line in "How to choose" ("choose carefully now"). | Medium. |
| Business models: support, open core, dual licensing; brand and trademark | Fireside chat; COSS panel | The COSS section now covers the idea. Add "open core" and "dual licensing" as two named examples if the group wants. Keep short. | Medium. Business detail is beyond this audience. |
| UC standard recommendation: BSD 3-Clause | Love Data Week deck p. 16 | Used. Expert should check against the UCLA discussion of BSD 3-Clause Clear. | |
| Choose a well-known license; SPDX identifiers | ABCs 24:00, 31:01 | Used. | |
| README template, citation file, Zenodo | Love Data Week deck | Used. | |
| Use the UC OSPO as the first contact; know a name in your TTO | COSS panel 23:49 | Add "find your TTO contact" as an action in the challenge. | High. Actionable. |
| The chart and guide are about 8 years old and may be refreshed | Tech transfer panel 37:47 | Keep the date caveat. | |

### Emerging topic: AI-generated code and licenses

In the 2026 education breakout, a speaker said non-permissive licenses may matter less if an AI agent can regenerate a package instead of reusing it. An audience member asked whether that is an accepted practice, and the speaker said he did not know. The fireside chat (36:06) also touched on AI models and license terms. This is contested and not settled law. Treat it as a note for the Episode 5 candidate or an instructor aside, not as lesson text. An expert should decide whether and how to teach it.

### Later episode (candidate)

A short episode on contributing to other people's projects:

* contributor license agreements and the developer certificate of origin (ABCs 17:43)
* use the project's license (tech transfer panel 41:30)
* red licenses and informed consent
* copying code from forums and AI-generated code (INTERSECT notes)

It fits as an Episode 5, after "Choosing a License". It also gives a home to the original Episode 4 objective about contributing.

### Glossary candidates

Public domain, source available, open core, dual licensing (exists), delegated authority (exists), contributor license agreement, developer certificate of origin, SPDX identifier, software bill of materials, due diligence.

## Expert flags found while reading

1. **Ownership.** The UC counsel on the tech transfer panel (12:00 to 14:00) says the 2021 UC copyright policy can leave ownership of scholarly works, including software, with the individual. This depends on whether the person is an academic author and whether the work is scholarly. The lesson says software is "typically owned by The Regents of the University of California" in Episodes 1 and 4, and the learner profile for Santiago says the same. Needs nuance. This is the most important correction.
2. **"Low risk" labels.** The chart summary in Episode 3 matches the speaker's colors, but he also says red licenses can be used with consent. Add that nuance.
3. **BSD 3-Clause versus 3-Clause Clear.** A UCLA officer said a switch is under discussion. Date: April 2026 panel.
4. **UC academic license.** The panels call it a non-commercial license that is not open source. Confirm the lesson wording.

## iASSIST 2026 handout (Tim Dennis)

"UC Open Source as Institutional Infrastructure", a one-page handout of prominent UC projects. It is a history and impact timeline and gives no licenses. It has no stated reuse license. The lesson paraphrases it with credit in comments. Used on 2026-11-12:

| Handout item | Episode | Use |
|---|---|---|
| tz database, 2011 lawsuit, public domain choice | Ep1 | Callout "A real case: the time zone database". Lawsuit details need a primary source. |
| BSD Unix, INGRES and PostgreSQL | Ep2 | One added paragraph in the BSD callout. |
| Jupyter, Spark, Ceph, EEGLAB, ChimeraX | Ep2 | Challenge "real UC projects". Licenses checked 2026-11-12, mostly from repository sidebars. |
| Spark and Ceph paths | Ep4 | Two examples in the COSS section. Verify the Spark donation and Ceph funding statements. |

Open issues in the handout: BSD Unix (1977) sits above INGRES (1973) in the timeline, and the footer cites a different Ruff video ID (eBriL3CDNeo) than the keynote scanned here (1VtGcD4fQLY).
