---
title: "Choosing a License"
teaching: 10 # teaching time in minutes
exercises: 15 # exercise time in minutes: think-pair-share 6, multiple choice 5, repository demonstration 4. Needs a pilot.
---

:::::::::::::::::::::::::::::::::::::: questions

- Who owns my code, and who decides how it is released?
- How do I choose a license that fits my goals and my institution's policies?
- How do I add a license to my project and tell people about it?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Determine who owns a piece of software and who must approve its release.
- Compare licenses against project goals and UC policy.
- Choose a license and explain which goals and constraints shaped the choice.
- Describe when commercial open source software (COSS) fits a project.
- Add a license file and a README license section to a repository.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: instructor

### Narrative outline: Santiago (draft for the group to edit)

- Santiago wrote a tool for a campus group as part of his job. A collaborator at another institution wants to use it.
- His question: who owns the code, and who approves a release?
- He checks with the technology transfer office.
- He picks a license from the UC-recommended list, then adds it to his repository and README.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: instructor

### Notes for the exercises

The exercises take about 15 minutes in total.

- Think, pair, share (6 minutes): learners work through Santiago's case. Two minutes to think, two to pair, two to share. Listen for the ownership question first and the license choice second.
- Multiple choice (5 minutes): three short scenarios, one per persona. Poll each, then ask one learner to explain the reason.
- Repository demonstration (4 minutes): show the steps on a demo repository. Learners with a GitHub account can follow along. Nothing here requires one.
- The scenarios and answers are drafts for the group to check. An expert should confirm the policy statements in the solutions.
- The slide deck also planned a matching exercise (license types matched to example projects). It is not built yet. It needs a list of projects and the criteria for a good match (issue #9).

::::::::::::::::::::::::::::::::::::::::::::::::

## Who owns the code?

Before you choose a license or decide to open source your software, determine who owns the code. That can be trickier than you would expect.

At the University of California:

- Software created using university resources is typically owned by The Regents of the University of California.
- Code created in connection with your research project or your staff position is typically owned by The Regents of the University of California.
- Grants may stipulate that the funder owns the results of the research, including code, or require a specific license.

You can learn more in the University of California's [copyright policy resources](https://copyright.universityofcalifornia.edu/). It is important to understand how the policy applies to your case. The resources explain details beyond the scope of this lesson.

## Work with your technology transfer office (TTO)

At UC, before releasing code under an open source license, you must check with your campus TTO. It is sometimes called the Office of Intellectual Property or Technology Commercialization.

The TTO will:

- verify ownership and funding requirements.
- make sure no third-party restrictions apply, for example from proprietary libraries.
- help you select the most appropriate license from the UC-recommended list.

## How to choose a license

The license you select will depend on your goals and on the policies of the University of California. Consider:

- who owns the code, and any funder requirements.
- how much reuse you want. Episode 2 compares permissive and copyleft licenses.
- the UC risk ratings for each license. Episode 3 summarizes the chart.
- the licenses of your dependencies. Episode 3 explains how they can clash.
- how familiar the license is. A well-known license is easier for other people, and their legal teams, to recognize and accept.

The Open Source Software chart and its companion guide can help you navigate UC policies and guide your discussion with your TTO.

Always consult your campus TTO before releasing UC-owned software.

<!-- Draft for the expert to check. The UC Love Data Week 2026 deck states this recommendation. A panelist at UC Open 2026 said UCLA may move to BSD 3-Clause Clear because of a debate about patent grants. -->

When you create a new repository, the UC OSPO standard recommendation is the BSD 3-Clause license. Your TTO still makes the final call.

## When is commercial open source an option?

<!-- Draft from the UC Open 2026 panel for Karla and the expert to check. -->

Some projects aim to become a business. Commercial open source software (COSS) is software that a company releases under an open source license while it earns money from something it does not give away, such as enterprise features, a hosted service, or support. Open source is the company's strategy. It is not the business model.

Ask these questions before you plan a COSS project:

- What are your goals? Many research teams do not want to start a company, and a standard open license is enough.
- What would customers pay for that you do not give away?
- Could a market support a business around this software?
- Have you talked to your TTO? Do it early, because ownership and funding terms can limit your options.

Some licenses limit commercial use. As Episode 2 explains, they are source available licenses, not open source licenses.

## UC resources

- [UC OSS Resources](https://security.ucop.edu/resources/open-source-software-licensing.html): resources and guides for open source activities at UC.
- [UC OSS Chart](https://security.ucop.edu/files/documents/resources/oss-chart.pdf) and [Companion Guide](https://security.ucop.edu/files/documents/resources/oss-chart-companion.pdf): UC guidance on license risks.
- [UC OSPO License Guide](https://ucospo.net/oss-resources/template-guides/license-guide/): guidance on institutional requirements and templates.
- [ChooseALicense.com](https://choosealicense.com): a tool for comparing license features. It does not supersede UC policies.
- [Making a COSS Play](https://www.youtube.com/watch?v=V4XjaDWG-cs) (UC Open 2026 panel, video): researchers, investors, and tech transfer officers discuss commercial open source.

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: choose a license for Santiago's tool

Santiago works as research staff at a UC campus. He wrote a data-cleaning tool for his campus group as part of his job. A collaborator at another institution wants to use it. He assumes the choice of license is his to make.

**Think (2 minutes):** On your own, answer these questions.

1. Who probably owns the code? Who must approve its release?
2. Use the chart summary in Episode 3. Which licenses are low risk for distributing outside UC?
3. Pick one license and give two reasons. Think about your goals, UC policy, and the license of any dependency.

**Pair (2 minutes):** Compare answers with a partner. Where you chose differently, explain your reasons.

**Share (2 minutes):** Be ready to report one reason from your pair to the group.

::::::::::::::::::::::::::::::: solution

1. At UC, code written for a staff position is typically owned by The Regents of the University of California. Santiago needs approval from his campus TTO before release.
2. In the 2018 chart, BSD and MIT are low risk in every situation. Apache 2.0 and MPL 2.0 can be moderate risk when you distribute modified code outside UC.
3. Answers vary. A good answer names a goal (for example, wide reuse), a UC constraint (for example, low risk in the chart), and a check of the licenses of any dependency.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: pick the best answer

Read each question. Choose the best answer, then compare with your neighbor.

**1. Camila** is a postdoctoral researcher at a UC campus. Her TTO has approved a release. She wants labs and companies to reuse her analysis scripts with as few conditions as possible. Which license fits best?

- A. BSD 3-Clause
- B. GPL 3.0
- C. PolyForm Noncommercial
- D. No license

**2. Valentina** leads a research software project at a UC campus. She wants a copyleft license, so that changes to her code stay open. She will share the code with collaborators outside UC. Under UC guidance, which license fits best?

- A. GPL 2.0
- B. GPL 3.0
- C. MIT
- D. BSD 3-Clause

**3. Santiago** wrote a tool as part of his staff job at a UC campus. A collaborator wants to use it. What should he do first?

- A. Add a BSD license and publish the code
- B. Ask the collaborator which license they prefer
- C. Check ownership and approval with his campus TTO
- D. Wait until the code has no known bugs

**4. Commercial open source.** Which statement best describes commercial open source software (COSS)?

- A. Open source software that you pay to download
- B. Software that a company releases openly while it earns money from a related product or service it does not give away
- C. Software with no license
- D. Open source software whose source code is hidden

::::::::::::::::::::::::::::::: solution

<!-- Draft answers for the group to check. An expert should confirm the policy statements. -->

1. **A.** BSD is permissive and low risk in the UC chart, and it lets companies and labs reuse the code. GPL 3.0 is high risk for distribution outside UC. PolyForm Noncommercial is not an open source license, and it blocks companies. With no license, nobody has permission to reuse the code.
2. **A.** GPL 2.0 is a copyleft license, and the UC chart rates GPL 2.x low risk. UC does not recommend GPL 3.0, because its patent provisions may conflict with UC policies. MIT and BSD are permissive, so they do not keep changes open. Valentina still checks with her TTO.
3. **C.** The university probably owns the code, so Santiago does not decide alone. A license choice comes after approval. The collaborator's preference does not change who owns the code.
4. **B.** COSS is a business strategy. The company shares some or all of the software under an open source license and sells something else, such as enterprise features, hosting, or support. Open source code is not hidden, and it does not have to cost money.

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## Add the license to a repository

After TTO approval, your instructor adds the BSD 3-Clause license to a demo repository. The steps are:

1. Navigate to the repository on GitHub.
2. Click **Add file** and then **Create new file**.
3. Name the file `LICENSE` (or `LICENSE.txt`).
4. Click **Choose a license template** and select **BSD 3-Clause License**.
5. Update the copyright holder to: The Regents of the University of California. In this scenario, the university owns the code, so this step matters.
6. Update the year to 2026.
7. Commit the file to the main branch.
8. Check that the repository now shows the "BSD-3-Clause" license badge in the sidebar.

GitHub automatically detects the `LICENSE` file and displays it in the sidebar. The beginning of the complete license file looks like this. The file keeps all terms from the template:

```output
BSD 3-Clause License

Copyright (c) 2026, The Regents of the University of California
All rights reserved.
```

If the badge does not appear, make sure the file is in the root directory and named exactly `LICENSE` or `LICENSE.txt`.

## Name the exact license

<!-- Draft for the expert to check. -->

Many license names cover several versions. BSD, for example, has 0-clause, 2-clause, 3-clause, and 4-clause forms. The Software Package Data Exchange (SPDX) project publishes a short identifier for each license, such as `BSD-3-Clause`. Use the identifier in your README and in a comment at the top of each source file:

```python
# SPDX-License-Identifier: BSD-3-Clause
```

The identifier is unique, easy for people to read, and easy for tools to scan. If you also publish a `CITATION.cff` file or archive your release on Zenodo, state the same license there.

## Communicate your license

After you add a `LICENSE` file, reference it in your README so users understand the usage terms right away. Add this section near the top of your README:

```markdown
## License

This project uses the BSD 3-Clause License. The [LICENSE](LICENSE) file contains the terms.
```

The [UC OSPO README template](https://github.com/UC-OSPO-Network/templates/blob/main/README.md) has a section for this. The license section names the license for people who encounter your README outside GitHub, for example on Zenodo, in email, or in exported PDFs. Include the `LICENSE` file when you share the project.

::::::::::::::::::::::::::::::::::::: keypoints

<!-- Draft from the episode text for the group to edit (issue #9). -->

- Find out who owns the code before you choose a license.
- At UC, check with your TTO before you release code under an open source license.
- Match the license to your goals, UC policy, and the licenses of your dependencies.
- Add a `LICENSE` file to the root of your repository and name the license in your README.

::::::::::::::::::::::::::::::::::::::::::::::::
