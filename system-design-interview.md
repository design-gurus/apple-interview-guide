# The Apple System Design Interview

Apple gives mid-level and senior candidates one design problem and 45 to 60 minutes to work through it. The question usually resembles a product that Apple already ships, such as file sync, media streaming, or push notifications. Four things are commonly reported as graded: scale, trade-offs, user experience, and security, and privacy counts as much as scale.

## Format

| Stage | Minutes | What you do |
|---|---|---|
| Clarify the problem | 5 to 10 | Agree on the features, the users, and the scale |
| Sketch the high-level design | 15 to 20 | Name the components and show how data moves |
| Go deep on two parts | 15 to 20 | Choose the storage layer and one other hard part |
| Close | 5 | Name the weak points and what you would fix next |

Entry-level candidates are commonly reported to receive coding rounds instead of this round. For senior roles, the design conversation is often framed around the team's own product.

## Questions commonly reported

| Question | What the interviewer tests | Lesson |
|---|---|---|
| A cloud file sync service like iCloud | Conflict handling, delta sync, offline devices | [Designing Dropbox](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-dropbox?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |
| A messaging system like iMessage | Message order, delivery to offline devices, encryption | [Designing Facebook Messenger](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-facebook-messenger?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |
| A media streaming service like Apple Music | Content delivery, caching, adaptive quality | [Designing Youtube or Netflix](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-youtube-or-netflix?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |
| Push notifications for phones | Fan-out, device tokens, delivery during bursts | [Designing a notification system](https://www.designgurus.io/course-play/grokking-system-design-interview-ii/doc/designing-a-notification-system?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |
| A mobile payment service like Apple Pay | Encryption, idempotent transactions, fraud checks | [Designing a payment system](https://www.designgurus.io/course-play/grokking-system-design-interview-ii/doc/design-payment-system?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |
| Photo storage and sharing | Large media storage, on-device processing, privacy | [Designing Instagram](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-instagram?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) |

Delta sync means sending only the parts of a file that changed. An idempotent transaction is one that has the same effect when it is submitted twice. Other reported questions include a device backup system, an online store, an app recommendation system, and a search engine on the device.

## What Apple's products imply

Apple ships products that one person uses on a phone, a tablet, a laptop, and a watch. Three themes follow from that fact.

- **Privacy.** State where data is encrypted, who holds the keys, and what stays on the device. In the messaging question, the server should not be able to read the message text.
- **Device limits.** The clients are phones with limited battery, storage, and network. A design that assumes a powerful client loses marks.
- **Sync across devices.** State how you detect that two devices changed the same item, and what the user sees when no safe merge exists.

A design that only scales well is reported as not a passing answer.

## What a strong answer includes

1. Written requirements before any diagram, including the offline and privacy requirements.
2. Rough numbers for storage and requests per second.
3. A reason for each component, and not only its name.
4. What the user sees when the network drops, and how the system recovers without losing work.
5. The failure of one service, one region, and one device.
6. A closing list of weak points, such as clients that were offline for weeks.

## The iOS design round

The iOS round is a client round and not a distributed systems round. You design one feature of one app on one device. The focus is on memory, concurrency, and the system frameworks. See [Roles](roles.md) for the details.

## Go deeper

- [Grokking the System Design Interview](https://www.designgurus.io/course/grokking-the-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview) teaches the method and the worked designs linked in the table above.
- Lesson: [System Design Interviews: A step by step guide](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/system-design-interviews-a-step-by-step-guide?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview), in Grokking the System Design Interview
- Lesson: [Strong vs Eventual Consistency](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/strong-vs-eventual-consistency?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview), in Grokking the System Design Interview
- Lesson: [What is Encryption?](https://www.designgurus.io/course-play/grokking-system-design-fundamentals/doc/what-is-encryption?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview), in Grokking System Design Fundamentals
- Free answer: [Apple system design interview questions and how to answer them](https://www.designgurus.io/answers/detail/apple-system-design-interview-questions?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=system-design-interview)
- Sibling free guide: [Apple system design interview page](https://github.com/design-gurus/grokking-system-design/blob/main/companies/apple.md) in the Grokking System Design repository
