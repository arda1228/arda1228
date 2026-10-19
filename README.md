# Arda Dogan

Full-stack software engineer in London with about two years of production experience. I mostly write TypeScript on NestJS and React, deployed to AWS.

**Open to new roles.** Email me at [ardadogan3334@gmail.com](mailto:ardadogan3334@gmail.com).

---

## Recent work

### Edify Systems · Full-Stack Software Engineer · Feb 2026 to present

- **Scheduled report emails.** I owned this feature end to end. AI-generated dashboards are rendered to PDF and emailed on a schedule. Each recipient gets one-click unsubscribe that meets RFC 8058, and a schedule pauses itself after repeated failures. I shipped it to production in stages over two weeks.
  <br>*NestJS · PostgreSQL · SQS · EventBridge · Terraform · React*

- **Date-range dashboards.** I built a shared date-token model so AI-generated charts can re-cut themselves to any period. The LLM writes parameterised SQL windows that get filled in at run time. I coordinated the 16-commit release across three engineers plus product and data, then ran the production promotion.
  <br>*NestJS · BigQuery · React*

- **Checklist follow-up engine.** I took this from the technical design doc through to delivery. Site managers can now enforce compliance workflows with configurable threshold triggers and manager escalation, without needing engineering help.

- **Production login loop.** About 15 customer accounts were stuck in a login loop that had been put down to caching. I traced the root cause to two frontend bundles sharing one Auth0 client's transaction slot.

- **Delivery reliability.** I made the deploy pipeline keep working when Sentry is down, since a Sentry outage could previously block every release. I also audited the Playwright suite and cut about 191 redundant tests to speed up CI.

### Kantar · Software Engineer · Sep 2024 to Feb 2026

- Built microservices for an event-driven survey platform on Express and Kafka, backed by Postgres and Redis. Throughput went up 40%.
- Led a dynamic traffic balancing feature that stops surveys from over-completing. It saved an estimated 20% in business costs.
- Designed an anti-corruption layer for a third-party partner's API and had the integration working in under 48 hours.
- Raised code quality standards with SonarQube (coverage of 80% or more) and automated Jest testing.

### Oracle · DevOps Intern · Jun 2022 to Jul 2023

- Built a data-masking utility in Go that automates log redaction to support GDPR compliance. Four teams adopted it.
- Worked as Incident Communicator for mission-critical cloud services during high-severity events.

---

## AI-augmented development

Claude Code is my main coding agent day to day. I use it with custom skills, hooks, MCP servers and parallel agents.

At Edify I set up the team's AI workflow:

- **Custom skills**, including a production-deploy workflow and our conventions for e2e tests and migrations
- **Hooks and pre-commit checks** that run on every change
- **MCP servers** connecting Linear, GitHub, Notion, Sentry and Slack
- **LLM eval harnesses** to measure prompt reliability. When failure rates wouldn't converge, I fixed the structure of the problem instead of tuning the prompt further.
- **Agent-built features.** Devin and a Claude-based bot built features from Slack requests, and I reviewed and shipped them.

I've also worked with the Claude Agent SDK, the Anthropic API and CodeRabbit.

---

## Projects

### [Busdoku](https://busdoku.com)
A daily 3x3 puzzle game about London bus routes, inspired by Tubedoku. I designed, built and deployed it on my own.

- **Data pipeline** that combines the TfL API with borough and Thames GeoJSON. Requests are disk-cached and retried, with concurrency capped to stay under rate limits.
- **Backtracking constraint solver** that requires all nine answers in a grid to be distinct.
- **Deterministic daily puzzles** generated on the client from a cyrb53 + mulberry32 seed, so no server is needed. This replaced the hand-authored puzzles and editor I started with.
- **Strict TypeScript**, with 116 passing tests across 14 files and 22 merged PRs over several months.
- Moved hosting from GitHub Pages to Cloudflare Pages, following a deploy spec I wrote. After launch I shipped a mobile bottom-sheet numpad, saved progress, a stopwatch and sharing. I also found and fixed several data-accuracy bugs.

### Cloud-Native Public Transport App
My university dissertation. It's a web app that encourages sustainable travel by pulling in data from external transport APIs. It runs serverless on Lambda and DynamoDB behind API Gateway, with infrastructure defined in AWS CDK. It was deployed live on CloudFront.
<br>*Python · TypeScript · AWS CDK · S3*

---

## Stack

- **Languages:** TypeScript · Python · Go
- **Backend:** Node.js · NestJS · PostgreSQL · TypeORM · Redis · Kafka · BigQuery · REST · event-driven architecture · Auth0/OAuth
- **Frontend:** React · TanStack Query · Zustand · Tailwind CSS · Zod
- **Infrastructure:** AWS (ECS, Lambda, SQS, EventBridge, S3, CloudFront) · Docker · Kubernetes · Terraform · GitHub Actions
- **Testing and observability:** Jest · Vitest · Playwright · TDD · Sentry

---

## Education

**BSc Computer Science, Loughborough University.** First-Class Honours (74%), July 2024.
<br>Highest module marks: Agent-Based Systems 99% · Operating Systems & Networks 87% · Formal Methods 84%

---

Open to full-stack and backend roles in London or remote. Email me at [ardadogan3334@gmail.com](mailto:ardadogan3334@gmail.com).
