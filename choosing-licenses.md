---
title: "Choosing a License"
teaching: 10 # teaching time in minutes
exercises: 2 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

<!-- wbcheck AI202: Instructors get no example projects, no criteria and no expected reasoning. They cannot judge whether the discussion has met its objective. -->

- Think, Pair, share: Think of an OSS project and roles ( contributor, researcher, commercial oss dev.), Discuss which license you would choose for that project and why.

::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::: questions 

<!-- wbcheck AI204: The episode has no explanatory text or worked example of choosing a license. Learners would be asked to match and justify licenses they have not been taught. -->

- Matching exercise: list various license types and projects, match licenses to OSS projects and discuss the pairings.

::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::: questions 

<!-- wbcheck AI202: The exercises are only described as plans and are placed in `questions` blocks. There are no actual scenarios, answer options or solutions, so nothing can be used for formative assessment. -->

- Multiple choice: Answers will be the different license types e.g. MIT, Apache 2.0, GPL etc.  Questions:  Project based scenarios...choose the best answer. Discuss answers. 

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

<!-- wbcheck AI202: None of the three planned exercises asks learners to decide whether a commercial open source model fits a project, so this objective is unassessed. -->

<!-- wbcheck AI206: 'COSS' is an uncommon acronym and is never expanded. Check whether the lesson's external glossary defines it. -->

- Compare key licensing factors for the type of OSS application (science/scholarship/non-commercialization) and list the options
- Choose an appropriate OSS license and explain the decision thinking when contributing to different projects
- Identify when a COSS is appropriate for OSS project.

::::::::::::::::::::::::::::::::::::::::::::::::

<!-- narrative anchor: Santiago (staff member, UC-owned code). His situation for this episode goes here: the tool he wrote for a campus group, who approves its release, and the license he then chooses. TODO (group), pending the persona decision in issue #12. -->

## Who owns the code?

Before you choose a license or decide to open source your software, determine who owns the code. That can be trickier than you would expect.

At the University of California:

- Software created using university resources is typically owned by The Regents of the University of California.
- Code created in connection with your research project or your staff position is typically owned by The Regents of the University of California.
- Grants may stipulate that the funder owns the results of the research, including code, or require a specific license.

You can learn more about the University of California's copyright policy at <https://copyright.universityofcalifornia.edu/>. It is important to understand how the policy applies to your case. There is more nuance than the slides can provide.

## Work with your TTO

Before releasing code under an open source license, you must check with your campus Tech Transfer office. It is sometimes called the Office of Intellectual Property or Technology Commercialization.

The Tech Transfer office (TTO) will:

- verify ownership and funding requirements
- make sure no third-party restrictions apply, for example from proprietary libraries
- help you select the most appropriate license from the UC-recommended list

## How to choose a license

The license you select will depend on your goals and on the policies of the University of California. The Open Source Software chart and its companion guide can help you navigate UC policies and guide your discussion with your TTO.

Always consult your campus Tech Transfer office before releasing UC-owned software.

## UC resources

- UC OSS Resources: resources and guides for open source activities at UC.
- UC OSS Chart and Companion Guide: the definitive list of UC-recommended "low-risk" licenses.
- UC OSPO License Guide: guidance on institutional requirements and templates.
- ChooseALicense.com: a tool for comparing license features. It does not supersede UC policies.

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: add a BSD license to your repository

After TTO approval, add the BSD 3-Clause license to your demo repository:

1. Navigate to your repository on GitHub.
2. Click **Add file** → **Create new file**.
3. Name it `LICENSE` (or `LICENSE.txt`).
4. Click **Choose a license template** and select **BSD 3-Clause License**.
5. Update the copyright holder to: The Regents of the University of California. This step is critical.
6. Update the year to 2026.
7. Commit the file to your main branch.
8. Verify: does your repository now display the "BSD-3-Clause" license badge in the sidebar?

::::::::::::::::::::::::::::::: solution

GitHub automatically detects the `LICENSE` file and displays it in the sidebar. Your file should look like this:

```output
BSD 3-Clause License

Copyright (c) 2026, The Regents of the University of California
All rights reserved.
```

If the badge does not appear, make sure the file is in the root directory and named exactly `LICENSE` or `LICENSE.txt`.

:::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::

## Communicate your license

After you add a `LICENSE` file, reference it in your README so users understand the usage terms right away. Add this section near the top of your README:

```markdown
## License

This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
```

This matters because users who read your README on platforms other than GitHub (Zenodo, email, exported PDFs) will see your license terms even without GitHub's automatic detection.

::::::::::::::::::::::::::::::::::::: keypoints 

<!-- wbcheck AI201: The keypoints come from a lesson-design / CLDT template. They say nothing about OSS licensing, so they cannot summarise or reinforce this episode's objectives. -->

<!-- wbcheck AI208: This keypoint is about choosing a lesson and data licensing, not software licensing. Learners reading the summary would be misled about the episode's topic. -->

- Using a narrative throughout a lesson helps reduce learner cognitive load
- Choosing a lesson includes considering data license and ethical considerations.
- Openly-licensed datasets can be found in subject area repositories or general data repositories.

::::::::::::::::::::::::::::::::::::::::::::::::
