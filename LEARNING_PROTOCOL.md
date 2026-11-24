# Learning protocol

## Source of truth

[CURRICULUM.md](CURRICULUM.md) identifies the canonical lesson IDs, issue links, learning sequence and prerequisites. The canonical issue's state and dated session comments are the learning record. The curriculum describes planned work; it does not prove mastery.

Count each canonical lesson once. Exclude duplicate, administrative, cancelled and superseded issues from mastery counts. In particular, #19 is an administrative duplicate of #17 and #20 is a duplicate of #18: leave both closed and use their canonical issues. A closed duplicate is never a completed lesson.

## Start and resume

1. Read README.md, CURRICULUM.md and this protocol. Use the curriculum's issue links; GitHub issue numbers and creation order do not define lesson order.
2. Retrieve canonical issue states and the relevant session comments. Include open and closed lessons when checking prerequisite evidence. Account for truncated search results; fetch a known issue directly when search results lack its current state or newly created issue.
3. Follow the learner's explicit choice first. Otherwise resume the latest actual learning session's recorded next step, including unfinished work on a deliberately selected later topic. If there is no session yet, use the first unfinished lesson whose prerequisites are satisfied. Administrative edits and audit comments never change the next lesson.
4. Read the candidate issue and its prior evidence before teaching. For previously demonstrated prerequisite objectives, reuse the evidence. For a missing prerequisite, ask a short independent diagnostic before deciding whether to teach it. Record any change of sequence.
5. State the current lesson ID, demonstrated knowledge, remaining gap and immediate next step. Keep one active lesson by default. If the record is ambiguous, ask the learner which unfinished topic to resume.

An unavailable or uncertain GitHub record is not evidence that a topic is new. Explain what cannot be verified. Never claim that progress was saved until the write succeeds.

## Teach without unnecessary repetition

Teach one concept at a time: the problem, mechanism, tradeoffs and a practical example. Ask one question at a time and wait for the learner's answer. Do not reveal an assessment answer before the learner attempts it. Use SAP/ABAP, AWS and full-stack examples when useful; identify Primer material and supplemental material.

Prior exposure is not mastery. A successful independent diagnostic may demonstrate an objective without reteaching it. Hinted, copied or assistant-supplied answers are practice, not independent evidence. Reassess them with a fresh prompt after feedback.

When a topic appears again in a new context, link the earlier evidence and assess only the new application or deeper objective. Intentional retrieval practice is recorded as a review of the original issue; it does not create a duplicate lesson or erase its history.

## Assess and close

Score a lesson's independent evidence out of 10:

| Dimension | Points |
| --- | ---: |
| Conceptual accuracy | 4 |
| Mechanism | 2 |
| Tradeoffs | 2 |
| Application | 2 |

The passing threshold is at least 8/10 **and every essential lesson objective demonstrated independently**. An overall score cannot compensate for an essential misconception. For a small practice question, give focused feedback or a provisional score; do not present it as full-lesson mastery. Multiple-choice guesses alone are insufficient.

Before closing a canonical lesson, record the actual questions or tasks, the learner's answer summary, assistance given, objective evidence, dimension scores and any remaining limitations. Check completion boxes only when their evidence exists. Then close as completed. Never close solely because reading was assigned, setup finished or an earlier chat mentioned the topic.

An open canonical issue may be unstarted, in progress, blocked or awaiting assessment; its latest session comment explains which. A closed canonical issue counts as mastered only with a passing assessment and no later unresolved essential gap. If that evidence is absent, clarify the record rather than infer success. Reopen the canonical issue when a demonstrated essential gap requires more work, preserving earlier assessments and explaining why. Do not reopen administrative duplicates.

## Record each learning session

Append a comment to the canonical issue before reporting that progress is saved. Use the learner's local date and timezone. Do not create learning-session comments for setup or audit work.

```markdown
## Learning session — YYYY-MM-DD (America/Los_Angeles)
- Lesson: SD-XX.XX (#issue)
- Mode: learning / diagnostic / assessment / deliberate review
- Status after session: in progress / blocked / awaiting assessment / mastered
- Covered: [specific objectives]
- Prompt(s) and task(s): [what the learner was actually asked]
- Learner evidence: [faithful summary; distinguish independent work from hints]
- Assistance: [none, or hints/answers supplied]
- Objective check: [demonstrated objectives and unresolved objectives]
- Assessment: accuracy X/4; mechanism X/2; tradeoffs X/2; application X/2; total X/10
  [Use "not assessed" or "provisional" when appropriate; never invent a score.]
- Gaps: [specific misconceptions or missing evidence]
- Next step: [one concrete action; lesson ID and issue link]
- Prerequisite/reused evidence: [links when applicable]
```

Update an existing comment only to correct an error, with the correction identified. Add new comments for new sessions so the learning history remains readable. If a save fails, retain the session summary in chat and disclose the failure.

## Completion and scope

Report demonstrated mastery, lessons in progress and planned scope separately. Setup counts and closed-issue totals are not learning progress. Count required and optional tracks separately if the curriculum distinguishes them. Review should be driven by recorded gaps or deliberate retrieval, not a fresh restart of the entire curriculum.

When asked to continue system design learning, consult this repository first and follow the resume rules above. This protocol describes actions taken during a learning session; it does not imply automatic monitoring or scheduled reminders.
