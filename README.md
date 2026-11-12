# LocalGraph Core

An embedded, zero-server graph memory engine for autonomous AI agents built with Relate by Neo4j[cite: 7, 8].

## Use case
Autonomous agents frequently suffer from context fragmentation and high-latency database roundtrips. LocalGraph Core provides an embedded, zero-latency relationship mapping engine that lives directly in-process or via file-backed storage, eliminating external server dependencies[cite: 8].

## How it uses Relate
* **Mode:** Single-file persistent directory mode (`./store`), ensuring data persists across reboots for judge inspection.
* **Why this mode:** Guarantees absolute data durability and zero-latency local relationship traversal without requiring remote database infrastructure[cite: 8].
* **Graph Models:** Stores agent execution context, memory nodes, and entity relationships locally, interacting via Cypher and the Neo4j ecosystem[cite: 8].

## Setup and run
1. Clone the repository:
   ```bash
   git clone https://github.com/rcortez056-spec/localgraph-core.git
   cd localgraph-core
