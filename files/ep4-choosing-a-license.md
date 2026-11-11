---
title: "Choosing a License (DRAFT from slides)"
teaching: 0
exercises: 0
---

<!-- Source: 2026-OSPO-licensing-presentation.pdf, the second paragraph of slide 7, and slides 8, 9, 16, 17, 18, 19 and 20. Text follows the slides. Wording fixes are limited to typos. -->
<!-- The slides put ownership and the TTO before the license types. This draft puts them first in Episode 4, so the capstone can ask who approves the release. The group can move them. -->
<!-- TODO (group): questions and keypoints are left for the cohort to write. Link targets on slide 17 were not in the text export; add them from the original slides. -->

:::::::::::::::::::::::::::::::::::::: questions

- TODO (group)

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

<!-- Objective below is from the Day 1 lesson design notes, not from the slides. -->

- Choose a license for an example project and explain why that is the right choice

::::::::::::::::::::::::::::::::::::::::::::::::

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

- TODO (group)

::::::::::::::::::::::::::::::::::::::::::::::::
