# Setup audit — 2026-11-24

Reviewed in America/Los_Angeles before the first learning session. This is a setup snapshot, not a live progress counter. Use canonical issue states and learning-session comments for later progress.

## Result

The revised curriculum has **148 canonical learning issues: 123 main and 25 optional**. All 148 were found open in the final live GitHub search, with titles and bodies matching the reviewed lesson specifications. The only two closed issues are administrative duplicates #19 and #20; both are excluded. **No lesson has been assessed or recorded as mastered by this setup work.**

The audit compared the upstream English [System Design Primer](https://github.com/donnemartin/system-design-primer) README (content blob SHA `9e2cdb88dec86c34c9b49b657f5629a1866c6976`) and relevant solution files with this repository's original README, curriculum, protocol and all issue bodies. The blob hash is a content fingerprint, not a commit identifier. [SOURCE_MAP.md](SOURCE_MAP.md) preserves the full comparison.

## Initial findings and repairs

| Initial finding | Repair |
| --- | --- |
| The curriculum listed 120 lessons, but only 119 canonical issues existed. | Created [SD-10.03 — High-level design and API contracts](https://github.com/PhoNoodles/system-design-learning/issues/122). Its earlier creation had not succeeded. |
| Refresh-ahead was absent. | Created [SD-07.11](https://github.com/PhoNoodles/system-design-learning/issues/123) and placed it before the caching assessment. |
| Two of the eight worked examples were absent. | Added [financial aggregation / Mint](https://github.com/PhoNoodles/system-design-learning/issues/124) and [social-network data structures / shortest-path traversal](https://github.com/PhoNoodles/system-design-learning/issues/125). |
| Most issue objectives were generic and reading links pointed only to broad sections. | Replaced all 119 original canonical issue bodies with specific objectives, an independent task, source classification, prerequisites and precise source links where the Primer covers the topic. |
| Several source topics were only implicit or mislabeled. | Made web-server/query/object caching, timeline search, reverse proxy versus load balancing, estimation references, MapReduce and scatter-gather explicit. Clarified that the worked key-value example is a query-result cache. |
| OOD and the additional practice bank were not represented. | Added seven optional OOD entries (six notebooks plus a clearly labeled circular-array placeholder extension) and sixteen optional design exercises. Reused suitable main-path issues to map all 23 named additional prompts. |
| Architecture and engineering-blog directories had no planned use. | Added two optional selected-reading activities. Their completion applies only to the recorded readings. |
| Primer material and original extensions were mixed together. | Classified every lesson and documented the boundary in the curriculum, issue body and source map. Detailed supplemental readings are verified when taught. |
| The curriculum had no canonical issue links or usable prerequisite graph. | Linked every lesson and prerequisite; preserved stable IDs and made row order explicit. |
| The old protocol could reopen closed administrative duplicates for lacking assessment evidence. | Restricted mastery/reopening rules to canonical lessons and explicitly excluded #19 and #20. |
| Resume behavior could lose a deliberately selected topic. | Prioritized the learner's choice, then the latest actual session's recorded next action, then the earliest ready unfinished lesson. |
| Related lessons could repeat the same explanation. | Separated foundations from deeper applications and required reuse of demonstrated evidence. |

**Changes:** 119 original canonical issues updated; 29 new canonical issues created; no existing learning issue closed or marked mastered. The new issues are the one previously missing lesson, three core coverage additions and 25 optional lessons. Existing IDs and evidence history were preserved.

## Verification performed

- Compared the full original curriculum with the original 121 issue records: 119 learning records and two administrative duplicates.
- Matched every one of the 148 final lesson IDs to one canonical GitHub issue, with no missing or extra open issue.
- Read each original issue immediately before updating it and stopped on unexpected changes. The reviewed originals were open with zero comments.
- Verified each write result and then fetched the complete open set using both creation-order directions to account for the connector's 100-result cap. All final titles and bodies matched the intended specifications.
- Confirmed the only closed issues remained #19 and #20, and directly verified their administrative duplicate state and reason.
- Checked every prerequisite exists, every prerequisite precedes its dependent in the displayed order, the graph has no cycles, and no main-path lesson depends on an optional lesson.
- Checked Primer README anchors against the fetched source headings; relevant solution files and the six OOD notebooks were read during the audit.
- Independently reviewed coverage and learning-memory rules before publication.

## Scope and practical limits

The source map accounts for the educational section structure, all eight worked system-design examples, six OOD notebooks, the circular-array placeholder, all 23 additional interview prompts, the under-development headings, the study guide, the starting resources and Anki decks. Source directories are indexed for selected reading. Project-administration sections such as translations, contribution instructions and contact information are intentionally not learning lessons.

The audit does not certify every external link, historical measurement or technical assertion in the upstream bibliography. Use current primary documentation or original papers when teaching supplemental or product-specific details. A curriculum mapping means planned coverage; it never establishes learner mastery.

## Starting point after this audit

[SD-01.01 — Performance vs scalability](https://github.com/PhoNoodles/system-design-learning/issues/1), with no recorded assessment. Before a later session, follow [LEARNING_PROTOCOL.md](LEARNING_PROTOCOL.md) and inspect live session records rather than relying on this dated snapshot.
