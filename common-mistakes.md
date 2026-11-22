# Common Mistakes in the Apple Interview

A vague project answer is reported to hurt more at Apple than a missed algorithm question. The ten mistakes below are specific to how Apple interviews: each team runs its own loop, each loop examines your own projects, and each design answer must address privacy. Every mistake has a direct correction.

## The ten mistakes

| # | Mistake | Round affected |
|---|---|---|
| 1 | Preparing for the company and not for the team | All |
| 2 | Not asking the recruiter what the loop contains | All |
| 3 | Practicing only algorithm problems | Domain |
| 4 | Guessing confidently in the domain round | Domain |
| 5 | Writing code that runs but is hard to read | Coding |
| 6 | Designing for scale and omitting privacy | System design |
| 7 | Assuming a powerful client | System design |
| 8 | Giving a correct design at the level below | System design |
| 9 | Telling team stories without your own part | Behavioral |
| 10 | Pressing a team for confidential detail | Behavioral |

## Preparation mistakes

**1. Preparing for the company and not for the team.** Each team writes its own questions. Read the job description, and prepare every technology that it names.

**2. Not asking the recruiter what the loop contains.** An Apple recruiter supports one team and usually gives a real answer. Ask how many rounds there are, what each covers, and which languages are expected.

**3. Practicing only algorithm problems.** Every loop is reported to include a project discussion. Prepare two projects to a depth of three follow-up questions, with decisions, constraints, and measurements.

## Technical mistakes

**4. Guessing confidently in the domain round.** The interviewer keeps asking why until you reach the mechanism. Saying "I do not know, and here is how I would find out" is reported to score better than a guess.

**5. Writing code that runs but is hard to read.** Names, edge cases, and memory use are all graded. State the plan, write the simple version, handle the empty input, and then improve the solution.

**6. Designing for scale and omitting privacy.** Privacy appears in almost every Apple design round. State where data is encrypted, who holds the keys, and what stays on the device.

**7. Assuming a powerful client.** Apple systems serve phones with limited battery, storage, and network. State what the user sees when the network drops and how work is recovered.

**8. Giving a correct design at the level below.** This is reported as the most common senior rejection. The components are right, but the answer has no failure cases, no offline behavior, and no way to switch the feature off.

## Behavioral mistakes

**9. Telling team stories without your own part.** Say what you did, in the first person, and give a measured result. Vague statements about alignment are reported to score badly.

**10. Pressing a team for confidential detail.** Teams describe roles in general terms and often cannot name the product. Ask precise questions about how the team works, and accept a general answer about what it builds.

## One smaller error

- Praising Apple products without saying how you use them. Name one product, one use, and one improvement.

## A check before the loop

1. You know the team, the round list, and the target level.
2. You hold one-page summaries of your strongest projects.
3. Every practice design states privacy, offline behavior, and failure.
4. Every story names your own actions and one measured result.

The [Four-week plan](four-week-plan.md) schedules each of these items.

## Go deeper

- [Grokking the System Design Interview](https://www.designgurus.io/course/grokking-the-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes) teaches the design method that prevents mistakes 6 to 8.
- Lesson: [Things to Avoid During System Design Interview](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/things-to-avoid-during-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes), in Grokking the System Design Interview
- Lesson: [Mid, Senior, and Staff Answers](https://www.designgurus.io/course-play/grokking-modern-mobile-system-design-interview/doc/mid-senior-and-staff-answers?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes), in Grokking Modern Mobile System Design Interview
- Lesson: [Context, Constraints, Choices, Results](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/context-constraints-choices-results?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes), in Grokking Staff Engineer Interview
- Free answer: [Apple vs Google interview: which one is harder?](https://www.designgurus.io/answers/detail/is-apple-interview-harder-than-google?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes)
- Free answer: [Does Apple ask LeetCode questions in interviews?](https://www.designgurus.io/answers/detail/does-apple-ask-leetcode-questions-in-interviews?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=common-mistakes)
