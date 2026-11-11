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

::::::::::::::::::::::::::::::::::::: instructor

### Narrative outline: Valentina (draft for the group to edit)

- Valentina wants to share part of her project and keep part closed.
- She installed packages through a package manager and has never checked their licenses.
- Her question: do the licenses of her dependencies allow what she wants?
- Needs from the group: a worked clash example and the compatibility rules.

::::::::::::::::::::::::::::::::::::::::::::::::

## A word of caution: dependencies

Your toolchain, IDE, or Python package manager may add packages and libraries to your application or code.

Make sure the licenses of those packages are compatible with each other, and that they let you accomplish what you want to accomplish.

## How UC rates the licenses of open source code you use

The University of California publishes a chart that rates open source licenses for using and redistributing open source code at UC.
The color for each license is intended to give "merely a high level assessment of the relative risk that use of a particular OSS license will violate UC Policies".
The chart does not compare licenses with each other.
All open source licensing of Regents-owned copyrights requires approval of the appropriate delegated authority, regardless of the risk category.

The chart sorts licenses into low, moderate, and high risk for two situations: using code inside UC, and distributing it outside UC. In short:

- Low risk in every situation: BSD, MIT, Apache 1.x (not 2.0 or later), GPL 1.x and 2.x, LGPL 2.x (not 3.0 or "any later version"), and the Educational Community License 2.0.
- Moderate risk in some cases of distributing outside UC: Apache 2.0 and the Eclipse Public License when you distribute modified code, and MPL 2.0 when you distribute modified code or code that only calls its functions.
- High risk for distributing outside UC: GPL 3.0 and LGPL 3.0 in every case, and AGPL 3.0 in every case except code that only calls its functions, which is moderate.
- Inside UC, the patent-granting licenses (Apache 2.0, Eclipse, MPL 2.0, AGPL 3.0, GPL 3.0, LGPL 3.0) are low risk if you add the required Internal Use Notice.

For any other open source license, contact the licensing office.

The full chart has every combination. See the University of California Office of the President [OSS Chart](https://security.ucop.edu/files/documents/resources/oss-chart.pdf) (4/17/18 version) and [OSS Chart Companion](https://security.ucop.edu/files/documents/resources/oss-chart-companion.pdf) (3/26/2018).

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

