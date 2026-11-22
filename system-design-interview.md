# Microsoft System Design Interview

One interview in the Microsoft loop is usually about design. It can be system design, which is the architecture of a whole service. It can also be low-level design, which means writing the classes for one component. Candidates at level 63 and above report more system design and less class design.

Ask which kind it is in the first minute. The two kinds need different preparation, and the hour is short.

## The two kinds of design round

| | System design | Low-level design |
|---|---|---|
| Typical level | 63 and above | Early-career and some mid-level loops |
| Reported questions | Chat service, file storage and sync, notification service, rate limiter, link shortener | Parking lot, elevator, file system |
| What is graded | Requirements, interface, data model, scaling, and failure handling | Class boundaries, correct state changes, and code that can be extended |
| Practice lesson | [Designing Dropbox](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-dropbox?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) | [Design a Parking Lot](https://www.designgurus.io/course-play/grokking-the-object-oriented-design-interview/doc/design-a-parking-lot?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |

## What Microsoft's products imply

Microsoft is reported to frame design questions around its own products. The table maps each product area to a practice lesson for a similar system.

| Product area | Reported question | Practice lesson |
|---|---|---|
| Teams chat | Design a chat service for millions of users | [Designing Facebook Messenger](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-facebook-messenger?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| OneDrive | Design file storage and sync with version history | [Designing Dropbox](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-dropbox?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Outlook | Design a web email service | [Design Gmail](https://www.designgurus.io/course-play/grokking-system-design-interview-ii/doc/design-gmail-rafay?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Outlook Calendar | Design a calendar with recurring events and time zones | [Design Google Calendar](https://www.designgurus.io/course-play/grokking-system-design-interview-ii/doc/design-google-calendar?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Notifications | Design a notification service for email, push, and text messages | [Designing a Notification System](https://www.designgurus.io/course-play/grokking-system-design-interview-ii/doc/designing-a-notification-system?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Azure API Management | Design an API gateway with routing and rate limiting | [Design an API Gateway](https://www.designgurus.io/course-play/system-design-interview-crash-course/doc/design-an-api-gateway?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Azure Blob Storage | Design storage for large binary files | [Design Amazon S3](https://www.designgurus.io/course-play/system-design-interview-crash-course/doc/design-amazon-s3?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |
| Short links | Design a link shortener with analytics and expiry | [Designing a URL Shortening Service](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-a-url-shortening-service-like-tinyurl?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) |

## What the interviewer looks for

Interviewers are reported to grade the order of the work. Requirements come first, then the interface, then the data model, then the parts that must scale. Expect follow-up questions about ten times the traffic and about which part fails first.

Three concerns are reported to matter more at Microsoft than at many other companies.

- **Enterprise security and compliance.** Many customers are banks, governments, and large companies. Cover encryption, identity, and access control without being asked.
- **Cost.** Explain where the design saves money, such as cheaper storage for files that are rarely read.
- **Multi-tenancy.** A tenant is one customer organization that shares the service with others. State how the design keeps each tenant's data separate.

Azure knowledge helps, but it is not reported to be required. You can describe the capability, such as "a globally replicated database", instead of naming a product. The tone is commonly described as collaborative, so think aloud and adjust the design when the interviewer gives feedback.

## What a strong answer includes

1. Functional and non-functional requirements, with numbers for users and traffic.
2. A short capacity estimate for storage and requests per second.
3. The API, then the data model, then a high-level diagram.
4. One or two deep dives, chosen with the interviewer.
5. Security, tenant isolation, and cost, raised without a reminder.
6. Trade-offs stated as a choice, with the option you rejected and the reason.
7. A failure review: what breaks first, and how the system recovers.

The lesson [System Design Interviews: A Step by Step Guide](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/system-design-interviews-a-step-by-step-guide?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview) teaches this order.

## Go deeper

- [Grokking the System Design Interview](https://www.designgurus.io/course/grokking-the-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview): the standard designs, including chat, file sync, and the rate limiter.
- Lesson: [Designing an API Rate Limiter](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-an-api-rate-limiter?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview), in Grokking the System Design Interview
- Lesson: [What is Authentication?](https://www.designgurus.io/course-play/grokking-system-design-fundamentals/doc/what-is-authentication?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview), in Grokking System Design Fundamentals
- Free article: [Microsoft system design interview questions](https://www.designgurus.io/blog/microsoft-system-design-interview-questions?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview)
- Free answer: [Top system design questions for the Microsoft interview](https://www.designgurus.io/answers/detail/what-are-top-system-design-questions-for-microsoft-interview?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=system-design-interview)
- Free guide: [Microsoft system design interview](https://github.com/design-gurus/grokking-system-design/blob/main/companies/microsoft.md) in Grokking System Design on GitHub
