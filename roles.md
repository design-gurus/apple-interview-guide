# How the Apple Loop Differs by Role

Every Apple team builds its own loop, so the role changes the interview more at Apple than at most large companies. The clearest difference is for iOS engineers, whose design round covers one feature on one device. Specialist teams replace part of the algorithm time with domain questions, and senior and manager roles add a round with a director.

This page covers only the roles that the source articles describe. Each detail is commonly reported and varies by team.

## Summary

| Role | What changes | What stays the same |
|---|---|---|
| iOS engineer | The design round is a client round on memory, concurrency, and frameworks | Coding rounds and behavioral questions |
| Specialist teams | Technical time moves to the team's own area | A project discussion in every loop |
| Senior and manager roles | A director round is added | The hiring manager owns the decision |

## iOS engineer

The iOS design round is a client round and not a distributed systems round. You design one feature of one app, running on one device. Agree on the scope aloud in the first minutes, because some teams want the client only and others want the client plus the interface to the server.

| Area | What to state |
|---|---|
| Local database | Core Data or SwiftData as the source of truth, so the screen works with no network |
| Networking | URLSession, and its background version for transfers that continue after the app leaves the screen |
| Background work | BGTaskScheduler asks the system for a short window; the system selects the time |
| Push | Apple Push Notification service; treat a push as a hint to fetch and not as guaranteed delivery |
| Concurrency | Which work runs off the main thread, which must stay free for drawing |
| Secrets | Tokens belong in the Keychain, the encrypted store that iOS provides |
| View layer | SwiftUI or UIKit, and how the view receives its data |

A workable budget for a 45 minute round is 5 minutes for requirements, 8 for the interface and data model, 10 for client architecture, 17 for the hardest part, and 5 for failure and release. At Apple the hardest part is often sync, memory, or concurrency.

Expect follow-up questions on low memory. State what you remove from the cache first and why. For images, decode a photo to the size of the view, because a full-size decode can use tens of megabytes.

A good practice subject is a note edited on a phone and on a Mac. Work through conflicts, offline edits, and retries.

## Specialist teams

Many teams spend the technical time on their own area. The reported examples follow.

- A camera team asks about image pipelines.
- A silicon team asks about hardware and memory.
- A services team asks about distributed systems.
- A systems team asks about concurrency, such as why a lock costs more than an atomic counter.

Language depth is also common. Swift, Objective-C, or C++ may be expected, depending on the team. The job description is the best available guide, so prepare every technology that it names.

## Senior and manager roles

Senior and manager loops usually add a round with a director. The director's review is reported to concern the level more than the ability to do the work. For senior engineers, expect at least one architecture conversation that is framed around the team's own product.

## Go deeper

- [Grokking Modern Mobile System Design Interview](https://www.designgurus.io/course/grokking-modern-mobile-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=roles) teaches the client round, with worked answers at mid, senior, and staff level.
- Lesson: [The Five Step Method and the 45 Minute Budget](https://www.designgurus.io/course-play/grokking-modern-mobile-system-design-interview/doc/the-five-step-method-and-the-45-minute-budget?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=roles), in Grokking Modern Mobile System Design Interview
- Lesson: [Sync and Conflict Resolution](https://www.designgurus.io/course-play/grokking-modern-mobile-system-design-interview/doc/sync-and-conflict-resolution?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=roles), in Grokking Modern Mobile System Design Interview
- Lesson: [Threading With Swift Concurrency and Coroutines](https://www.designgurus.io/course-play/grokking-modern-mobile-system-design-interview/doc/threading-with-swift-concurrency-and-coroutines?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=roles), in Grokking Modern Mobile System Design Interview
- Free answer: [Apple iOS system design interview expectations](https://www.designgurus.io/answers/detail/apple-ios-system-design-interview-expectations?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=roles)
- Sibling free guide: [Mobile system design interview](https://github.com/design-gurus/mobile-system-design-interview)
