# java-internals-concurrency-lab

Core Java internals and concurrency: HashMap, race conditions, executors. Java 21, Maven, JUnit 5.

Part of the [java-fullstack-ai-engineering-hub](https://github.com/mahendrashongunti/java-fullstack-ai-engineering-hub). Working rules are in the hub's `AGENT.md`; progress is tracked only in the hub's `REPO_LIST.md`.

## Challenges

| # | Challenge | Evidence and notes |
|---|---|---|
| A1 | HashMap internals | [docs/a1.md](docs/a1.md) |
| A2 | Race condition lab | [docs/a2.md](docs/a2.md) |
| A3 | Executors and CompletableFuture | [docs/a3.md](docs/a3.md) |

## Conventions

- Failing or naive code is kept next to the fix (`Naive` suffix, `@Disabled` or the `break-it` profile).
- Two commits per challenge: `aN: reproduce ...`, then `aN: fix ...`. Tag `aN-done` when verified.
- No secrets in Git. Copy `.env.example` to `.env` where one exists.

## Run

```bash
mvn test
```

If Maven fails with an unsupported class file version, build with JDK 21 (`JAVA_HOME` pointing at it).
