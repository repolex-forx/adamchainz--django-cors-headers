# Repolex Knowledge Graph of adamchainz/django-cors-headers

RDF knowledge graph data for [adamchainz/django-cors-headers](https://github.com/adamchainz/django-cors-headers), parsed by [repolex](https://repolex.ai).

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
rlex download adamchainz/django-cors-headers
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8d96f0172cfa611124c4dc6eee14ee4a45e67589
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 8d96f0172cfa611124c4dc6eee14ee4a45e67589
│           └── chunk-001.nq.gz
├── blob
│   ├── 06e257a52d435dc944f3e752c9fcdb5dac1260b8.nq.gz
│   ├── 0806c05c4e8f70e4f022f80383e5aa502924a1b4.nq.gz
│   ├── 098c2019f9c97a6ac7f037d9f9e72a45ebfc71f6.nq.gz
│   ├── 205ab9ad9df4ab629d1b7b8d8a72b41f44d8824c.nq.gz
│   ├── 22ddbb118475b52ce8ecba56d9ec45009923da58.nq.gz
│   ├── 2599b0b53d26a0f76f24fcf27f57530b6e11250b.nq.gz
│   ├── 2a7f84f54867d02714727f82eef95d3be939d666.nq.gz
│   ├── 3ba13e0cec6cbbfd462e9ebf529dd2093148cd69.nq.gz
│   ├── 40f4ac757715bb1a8c355eda9124141fdda3aeff.nq.gz
│   ├── 438d629c3ce988e3afffa71110b9660853d38549.nq.gz
│   ├── 621fa306edca291eb8617aa515dfc86902cc9caa.nq.gz
│   ├── 6305fca317e61ecd7674489a82107ece95ca4666.nq.gz
│   ├── 68df125cd506140f1a4747eefdc2a4400b7c4271.nq.gz
│   ├── 6b7c68f7b91302b7e134d732bc020974c23d5732.nq.gz
│   ├── 83629f3a1382388ac43f11a2ae8cfc7ede5cb2a1.nq.gz
│   ├── 87c0c4466c17a4430267c80a495bbde3da553e4a.nq.gz
│   ├── 93acb639926ccf42e9a2f76f02419eeaf0405c3a.nq.gz
│   ├── 943b9c066eabdd85adecb35fd1e309b31e5f6ed9.nq.gz
│   ├── 97d8951bdce1a4f6111b5a607451db32d3248772.nq.gz
│   ├── 9e7160e921c3fcb75030788cb3cf5aac1280d2fc.nq.gz
│   ├── a790fb1d2f54d72bfd262c959e899c306fa1c0f3.nq.gz
│   ├── b69a7309931306d54ac2f3aafe8a49b660e8d86c.nq.gz
│   ├── be5ff97e8f517ea6be134cec01686ca0a19eb92e.nq.gz
│   ├── bf738faebaebd634315d3749605de1eec21b4362.nq.gz
│   ├── c2f08ab667b79ff43ece76ae0a6298c4748f2945.nq.gz
│   ├── c47287e167a3b95c5f3469e972f66a9b488056cb.nq.gz
│   ├── cb8393b6f68f3d5088b4dd783998f4f293ec7ddb.nq.gz
│   ├── cc29d43e0a5ab969ccff8e35db06dc73cd4a016a.nq.gz
│   ├── dea0450b9829c75c1a4e0bf11c38488d54aaea7d.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ec8cb0966cef37e50f5adfb674a87501e1e67e2f.nq.gz
│   └── f43975e4bd7c611037cfc28f86203b4f99248259.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8d96f0172cfa611124c4dc6eee14ee4a45e67589.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 40 files
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

[adamchainz/django-cors-headers](https://github.com/adamchainz/django-cors-headers)

---
*Parsed on 2026-10-15 by [repolex](https://repolex.ai)*
