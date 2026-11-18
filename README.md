# LocalGraph Core

An embedded graph memory engine for autonomous AI agents, built on Relate by Neo4j.

## Use case

Agents often lose context between steps and waste time on repeated database round trips. LocalGraph Core keeps relationship data in-process or in a local file, so agents can query it without a separate database server.

## How it uses Relate

- **Storage:** [Confirm: single-file store at `./store`, or a directory store]
- **Persistence:** [Confirm: data survives restarts. State exactly what is true, e.g. "writes are flushed to disk before returning"]
- **Graph models:** Stores agent execution context, memory nodes, and entity relationships, queried with Cypher.

## Limitations

- [Confirm and list: e.g. "No crash-recovery guarantee for writes interrupted mid-operation" or "No backup or snapshot tooling yet"]
- Not a replacement for a production database server.

## Setup

```bash
git clone https://github.com/rcortez056-spec/localgraph-core.git
cd localgraph-core
```
