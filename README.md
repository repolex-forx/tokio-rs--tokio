# Repolex Knowledge Graph of tokio-rs/tokio

RDF knowledge graph data for [tokio-rs/tokio](https://github.com/tokio-rs/tokio), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download tokio-rs/tokio
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│   ├── lsp
│   │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│   └── repolex
│       └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
├── blob
│   ├── 0b08695a1c0c6094c2f2f0e29e5472d47f9d8843.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 28e630cf40d23e85e1b1c48eea4c7c2e8afd90f9.nq.gz
│   ├── 3927b25f95c557ac338e946f43a251fa28a29a64.nq.gz
│   ├── 3a67db789eb725ce45c83528ff6fa4c50b88f810.nq.gz
│   ├── 491ff56f9400566458292b0956099dcf6360e1ad.nq.gz
│   ├── 6bc5d49f2c3e2df66c16ec6d0a6c828bf0867d21.nq.gz
│   ├── a9d37c560c6ab8d4afbf47eda643e8c42e857716.nq.gz
│   ├── ae67cac17bd32933fc3da519e2ba7e8585964faf.nq.gz
│   ├── b7bb3fb7329e43989b33dcfb127fabf1a066ad61.nq.gz
│   ├── d686c27e57bd94899b9fe7eadc9dfa94b061f5c0.nq.gz
│   ├── da8c81272b4d0bde1b282ea8f6cfb355bb203150.nq.gz
│   └── f6e61d2bbfb318ac1d6fd6c78d4a432deb129345.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
├── files
│   └── tokio-rs
│       └── tokio
│           ├── aggregate
│           │   ├── ast
│           │   │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│           │   ├── dataflow
│           │   │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│           │   ├── lsp
│           │   │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│           │   └── repolex
│           │       └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│           ├── blob
│           │   ├── 0b08695a1c0c6094c2f2f0e29e5472d47f9d8843.nq.gz
│           │   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│           │   ├── 28e630cf40d23e85e1b1c48eea4c7c2e8afd90f9.nq.gz
│           │   ├── 3927b25f95c557ac338e946f43a251fa28a29a64.nq.gz
│           │   ├── 3a67db789eb725ce45c83528ff6fa4c50b88f810.nq.gz
│           │   ├── 491ff56f9400566458292b0956099dcf6360e1ad.nq.gz
│           │   ├── 6bc5d49f2c3e2df66c16ec6d0a6c828bf0867d21.nq.gz
│           │   ├── a9d37c560c6ab8d4afbf47eda643e8c42e857716.nq.gz
│           │   ├── ae67cac17bd32933fc3da519e2ba7e8585964faf.nq.gz
│           │   ├── b7bb3fb7329e43989b33dcfb127fabf1a066ad61.nq.gz
│           │   ├── d686c27e57bd94899b9fe7eadc9dfa94b061f5c0.nq.gz
│           │   ├── da8c81272b4d0bde1b282ea8f6cfb355bb203150.nq.gz
│           │   └── f6e61d2bbfb318ac1d6fd6c78d4a432deb129345.nq.gz
│           ├── branch
│           │   └── branch.nq.gz
│           ├── commit
│           │   └── commit.nq.gz
│           ├── filetree
│           │   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
│           └── tag
│               └── tag.nq.gz
├── filetree
│   └── 6847ed76ce77eb9fba10bf954c23058c6949d463.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

26 directories, 44 files
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

## Source repository

[tokio-rs/tokio](https://github.com/tokio-rs/tokio)

---
*Parsed on 2026-03-21 by [repolex](https://repolex.ai)*
