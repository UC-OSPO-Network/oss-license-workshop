---
title: "When Licenses Clash"
teaching: 20
exercises: 10
---

::::: questions
 - What are dependencies
 - What happens if my dependency has a license different from my project license
::::::

:::::: objectives
<!-- wbcheck AI202: No exercise asks learners to identify dependencies. The only challenge gives them the dependency licenses directly, so this objective is never assessed. -->

 - Identify dependencies
 - Determine if the licenses in my project are compatible
::::::

<!-- wbcheck AI204: The episode has no explanatory text. It does not define a dependency, does not explain permissive versus copyleft licenses, and does not show a worked example before learners are asked to judge com... -->

<!-- narrative anchor: Valentina (researcher, partial release). Her situation for this episode goes here: the project she wants to share in part, and the package whose license might clash. TODO (group), pending the persona decision in issue #12. -->

## A word of caution: dependencies

Your toolchain, IDE, or Python package manager may add packages and libraries to your application or code.

Make sure the licenses of those packages are compatible with each other, and that they let you accomplish what you want to accomplish.

## How UC rates the licenses of open source code you use

The University of California publishes a chart that rates open source licenses for using and redistributing open source code at UC.
The color for each license is intended to give "merely a high level assessment of the relative risk that use of a particular OSS license will violate UC Policies".
The chart does not compare licenses with each other.
All open source licensing of Regents-owned copyrights requires approval of the appropriate delegated authority, regardless of the risk category.

Table: Risk ratings for internal use at UC, by license (UC OSS Chart, 4/17/18 version)

| License | Flags | Unmodified | Modified |
|:------------------------------------------------------------------|:-------|:-----------------------------|:-----------------------------|
| BSD (must retain the copyright notice) | none | Low | Low |
| MIT (must include the original copyright notice) | none | Low | Low |
| Apache 1.x, not 2.0 or later (must reproduce the original copyright notice) | none | Low | Low |
| GPL 1.x or 2.x, or LGPL 2.x, but not 3.0 or "any later version" | H | Low | Low |
| Educational Community License 2.0 | PG, H ** | Low | Low |
| Apache 2.0 | PG, H ** | Low, with Internal Use Notice | Low, with Internal Use Notice |
| Eclipse Public License 1.0 and 2.0 | PG, H | Low, with Internal Use Notice | Low, with Internal Use Notice |
| MPL 2.0 | PG, H | Low, with Internal Use Notice | Low, with bug fixes only |
| Affero GPL (AGPL) 3.0 | PG, H | Low, with Internal Use Notice | Low, with Internal Use Notice |
| GPL 3.0 or LGPL 3.0 | PG, H | Low, with Internal Use Notice | Low, with Internal Use Notice |

Table: Risk ratings for external distribution outside UC, by license (UC OSS Chart, 4/17/18 version)

| License | Unmodified | Bug fixes | Otherwise modified | Function calls only |
|:------------------------------------------------------------------|:---------|:---------|:-----------|:-----------|
| BSD | Low | Low | Low | Low |
| MIT | Low | Low | Low | Low |
| Apache 1.x, not 2.0 or later | Low | Low | Low | Low |
| GPL 1.x or 2.x, or LGPL 2.x, but not 3.0 or "any later version" | Low | Low | Low | Low |
| Educational Community License 2.0 | Low | Low | Low | Low |
| Apache 2.0 | Low | Low | Moderate | Low |
| Eclipse Public License 1.0 and 2.0 | Low | Low | Moderate | Low |
| MPL 2.0 | Low | Low | Moderate | Moderate |
| Affero GPL (AGPL) 3.0 | High | High | High | Moderate |
| GPL 3.0 or LGPL 3.0 | High | High | High | High |

For any other open source license, contact the licensing office.

If you use software internally within UC under a patent-granting license such as GPL 3.0, with no intention of external distribution, you must add the required Internal Use Notice.

PG means a "patent-granting" license. H means a "hereditary" license, sometimes called viral.
** The heredity requirement may be overridden for derivative works under section 4 of Apache 2.0 and ECL 2.0. You can add your own copyright statement to your modifications.

Source: University of California Office of the President, [OSS Chart](https://security.ucop.edu/files/documents/resources/oss-chart.pdf) (4/17/18 version) and [OSS Chart Companion](https://security.ucop.edu/files/documents/resources/oss-chart-companion.pdf) (3/26/2018).
<!-- EPISODE CONTENT HERE -->

::::::: challenge
<!-- wbcheck AI202: The instructions contain typos ('Place and X is there is'). The grid also gives no guidance for nuanced cases such as LGPL linking, Apache-2.0 into GPLv2, or proprietary terms, where the answer is... -->

Mark an X in each cell where there is a conflict. Leave the cell empty if there is no conflict.

<!-- wbcheck AI208: The table is tab-separated plain text, not a Markdown pipe table, so it will render as a jumbled paragraph. The header also splits 'Dependency License' across lines, and the 'Commercial' row is tru... -->

| Dependency license | BSD | MIT | Apache | LGPL | GPL | Commercial |
|---|---|---|---|---|---|---|
| **BSD** | | | | | | |
| **GPL** | | | | | | |
| **Commercial** | | | | | | |

Read each row as the license of the dependency and each column as the license of **My project**.

::::::

:::::: keypoints
<!-- wbcheck WB112: `keypoints` still has placeholder bullet text: "keypoint 1" -->

 - keypoint 1
 - keypoint 2
::::::

