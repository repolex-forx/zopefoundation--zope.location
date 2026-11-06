# Repolex Knowledge Graph of zopefoundation/zope.location

RDF knowledge graph data for [zopefoundation/zope.location](https://github.com/zopefoundation/zope.location), parsed by [repolex](https://repolex.ai).

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
rlex download zopefoundation/zope.location
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 049b80b8f87ff51e3eb31f25aa8fa1e43a614fb0
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 049b80b8f87ff51e3eb31f25aa8fa1e43a614fb0
│           └── chunk-001.nq.gz
├── blob
│   ├── 034043e1628b277e8c3805e50acd2ac1e6e85255.nq.gz
│   ├── 0a3c26bebbff60b1fd2697ca28337f865c453625.nq.gz
│   ├── 0ab12fe1e0c8eb6cb0d68fce1b14a2209cdb0def.nq.gz
│   ├── 0c1694becee4b0e81c65815f65fb931ae17afaf1.nq.gz
│   ├── 149e0f19635a924a1aa7d0447ef6e9cf9142ce82.nq.gz
│   ├── 1f321f52abb7db6f79c285bab56e2852dc575699.nq.gz
│   ├── 1f4607781b17338521801e3544f341ad74ee5859.nq.gz
│   ├── 2022a56530f4c3b9afb427954f27ad5f280877bc.nq.gz
│   ├── 35599fb206e05dc7aca0db979e3fc815a7267910.nq.gz
│   ├── 39089817a5126c64cb1565f9ad93e8c91c05e8ac.nq.gz
│   ├── 390ba286f1ca3ef0022a56594a8e98a64d6462a1.nq.gz
│   ├── 4726b1dde4f314bb04f856473dff006933577b60.nq.gz
│   ├── 4ac2ed2361b34a3de45d54432da7ba49e32faf02.nq.gz
│   ├── 4c19709d342491dfc4296d40e7c79a23d4c63921.nq.gz
│   ├── 5bb534f795ae0f566ba9f57c31944d8c6f45284c.nq.gz
│   ├── 5d035ba1e25f6663e51012b0e64d8415739ea04c.nq.gz
│   ├── 5e2f002e3a47299c2b8590f215376ab3230f4606.nq.gz
│   ├── 5eb71fee0e4451c06c18a7c1266ddadf608aa010.nq.gz
│   ├── 5f1bf4fe952d3b212a157e836be92c7c82c0d8e5.nq.gz
│   ├── 6358cbba00629574df9a1e215e6b4acf3e06a7cc.nq.gz
│   ├── 6c18313ac5aae10eabd6943b9798b805fda4ca99.nq.gz
│   ├── 717bb607f8a664ec726e9216cbe5c07025598268.nq.gz
│   ├── 71fea5a2b1a22847565760405920dea246b3f258.nq.gz
│   ├── 79859e06010bf4967c5b4b044afea6ef39742938.nq.gz
│   ├── 94b3ce53dbc9ab708230323306fdfb757ad5f8b8.nq.gz
│   ├── a6c3bf91ada078468ed814a009e269686dbd78b5.nq.gz
│   ├── a9e4e0c2d19a56fe040950eddae829faefe3601f.nq.gz
│   ├── bf28b3f880e410ebb7f8c6e4b3aeb618784dcf42.nq.gz
│   ├── c31d815db6949c1387483bf2bde9677004f16f28.nq.gz
│   ├── c5508b9f083362a81185d598327e7801d837cb18.nq.gz
│   ├── ca0e267300ffe62b2c120455300570bf5bf7c90b.nq.gz
│   ├── ccdedc28073a0ba8303c52c91284a4e7e70bb471.nq.gz
│   ├── d01d75fb06fc0c982d151ea2150422446e535d61.nq.gz
│   ├── dad64f88ce982e194ad18a138be3738a169fbef0.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e2303fbaa0c001111f05f10159c5c3531f4c91aa.nq.gz
│   ├── e3579011e1a5792ed2adb52fe79f1ac001b9c3bf.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f0ed9d001e553f388470f3a0b5eca7e9269311c7.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 049b80b8f87ff51e3eb31f25aa8fa1e43a614fb0.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 47 files
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

[zopefoundation/zope.location](https://github.com/zopefoundation/zope.location)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
