# Repolex Knowledge Graph of canonical/s3-integrator

RDF knowledge graph data for [canonical/s3-integrator](https://github.com/canonical/s3-integrator), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download canonical/s3-integrator
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 64daa19fceb3c296557c67fbf65a59a9e4cfc1e1
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 64daa19fceb3c296557c67fbf65a59a9e4cfc1e1
│           └── chunk-001.nq.gz
├── blob
│   ├── 03b6c62c3b4b6a3ea973d906ced2d252a7295438.nq.gz
│   ├── 064d2780a92a6a947320030918921d09c93818af.nq.gz
│   ├── 0873cfd4d3b7264845c7f9bb65a8e65abb59695a.nq.gz
│   ├── 0b406b6a5a1082f7657d3d6796afdf98e1746f01.nq.gz
│   ├── 0f5b60744805a5db19be91ad6e8d6b731f84b095.nq.gz
│   ├── 104af57e813b41d3cf230b6f12f2c877ca7ddb41.nq.gz
│   ├── 150eb98ff2cc1ed1add1e91b83b75541248df13b.nq.gz
│   ├── 1e27e188674ba0bf6986afc2a61da18aef4cdde8.nq.gz
│   ├── 261e4bae1ec3a2234f0fc1bd1f468c10dc157b44.nq.gz
│   ├── 2b3ae78fb726a4124be96a71cbfcb9721b448bd0.nq.gz
│   ├── 2fcf6e5b6533939cfeb42aa864763b8d8864cd87.nq.gz
│   ├── 30dbc82cf2670bf734c8fc8764980338a274324a.nq.gz
│   ├── 3d498ded5589609ea4c1254f27c996b5a795f913.nq.gz
│   ├── 46e0665e5c9cbad9d280bf48060b7644d93b68c8.nq.gz
│   ├── 4a9535be1242e3077ecadf63003c2b3fbfb6ae73.nq.gz
│   ├── 56e16842d4a876f35e96dd88cc440514cac946d9.nq.gz
│   ├── 683178fb291e0b775b735b15ade85ab6c88220d3.nq.gz
│   ├── 7347b7c599f7c24b41f2c9637e06f06f7faa5f62.nq.gz
│   ├── 772d23619d149ab4ef283d8f70187f1f0e9e7ec7.nq.gz
│   ├── 81c6f28f9a599db64b3c3fd745a345dde7e86c65.nq.gz
│   ├── 8da6fe3f84af441c81635a8ee33a1529ee0dfecb.nq.gz
│   ├── 8fe80688a444c5181ab2c77753733ad24fb6c982.nq.gz
│   ├── 90236665a0ab74cc9c6371ac2b4024f3df7b2d5f.nq.gz
│   ├── 92d1f510cc31f1702aa37e5002641ef522eac624.nq.gz
│   ├── 98946f819f5f0666d4823b67218a46b5a1b6483a.nq.gz
│   ├── 98e4595d9ed5fc2455b43e922cb4c5c73ee109e1.nq.gz
│   ├── 9a70a2deb7eb501a89805a7f6e8d9550883b2098.nq.gz
│   ├── a587214d30e85f6fb2ffde59bacfc355289ceed8.nq.gz
│   ├── b0712be2bc8f236aaf43efb0f50f216154f46606.nq.gz
│   ├── b0fbb34478f1fbab8cd4e79f0f42987afbf911aa.nq.gz
│   ├── b87aef544c96c7de92ac6a7603a1127ca8efe399.nq.gz
│   ├── ba1760c62ef0e7fb23b8121e693da9f1392a1514.nq.gz
│   ├── c1c5dda94735328223d8ef2671820eddd686ce47.nq.gz
│   ├── c4d4c799deb8bcc3c247d5c39fb0f1d96bea7166.nq.gz
│   ├── cf069ab2e31e0bc00e91379b7b654734cb6bc72e.nq.gz
│   ├── d645695673349e3947e8e5ae42332d0ac3164cd7.nq.gz
│   ├── d88f4a06fea2f9a8e4df6fbe3d01c16877fa9efa.nq.gz
│   ├── db3bfe1a652400bb6963dfc7ede76820781ee928.nq.gz
│   ├── dbf4d5bb721e2c91fc81ad9e7bc352896740ad17.nq.gz
│   ├── e2052934adade689ffa7d2121365b89efe858afc.nq.gz
│   └── f96f6c7dbac54f77c4b266d3a79e494bd3fef7e6.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 64daa19fceb3c296557c67fbf65a59a9e4cfc1e1.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[canonical/s3-integrator](https://github.com/canonical/s3-integrator)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
