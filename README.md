# keel plugin: keel Product

Initiatives, teams and product docs, from idea to the teams' stories, with their own workflows and agents. Beta.

> **Status: planned.** The code still lives in [keel-v2](https://github.com/MiladNalbandi/keel-v2). It moves here step by step, as
> [the plugin plan](https://github.com/MiladNalbandi/keel-v2/tree/main/docs/plugins) says. There is nothing to install yet.

| | |
| --- | --- |
| id | `product` |
| needs | keel core (plugin SDK 1), Tasks, Jira |
| works with | — |
| parts | engine · api · web · content · migrations |
| trust level | runs code in keel |

**What it adds to keel**

- the Initiatives and Teams pages
- 5 product workflows and 4 agents

**Where the code is today (keel-v2)**

- product/ in keel-v2 (already an add-on)

## Layout

```
keel-plugin.yml   the manifest
engine/           Python package for keel's engine
api/              Kotlin, a thin Spring Boot jar
web/              React pages and slots (an ES module)
content/          workflows, agents, skills, commands
migrations/       its own database tables (own Flyway history)
```

## Install

When it is released: in keel, **Control › Plugins › Marketplace › keel Product › Install**. keel checks the file's
signature, shows what the plugin may do, and asks you before it installs.

## License

MIT
