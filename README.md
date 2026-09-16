# Repolex Knowledge Graph of json5/json5

RDF knowledge graph data for [json5/json5](https://github.com/json5/json5), parsed by [repolex](https://repolex.ai).

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
lexq download json5/json5
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c3a75242772a5026a49c4017a16d9b3543b62776
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── c3a75242772a5026a49c4017a16d9b3543b62776.nq.gz
│   └── repolex
│       └── c3a75242772a5026a49c4017a16d9b3543b62776
│           └── chunk-001.nq.gz
├── blob
│   ├── 00ee7939c4e40d456f9d10d65d9861a701cc2f0a.nq.gz
│   ├── 1123c534520d9b23d50bf56256518b357ef5b1dd.nq.gz
│   ├── 1c45bca5876aa88b947b4ae32b85f23e64aa1143.nq.gz
│   ├── 215ccd843abc25c3805ed9307f813f046dcb1459.nq.gz
│   ├── 2171aca5a833acbc6fb2b402433d8f10ff95c73f.nq.gz
│   ├── 29da2850676198c94659ce28eaa439a36476ef5b.nq.gz
│   ├── 2eaadb6531df2290e203fd4a4942bfb39492c6b5.nq.gz
│   ├── 322bed5576031badba3383fe7343d39d21292942.nq.gz
│   ├── 36796388892da3dc8cfecd4168d4368aa01edfe1.nq.gz
│   ├── 3aa29bee0344ef9a7c800ccc7a1fd71c55ade4a0.nq.gz
│   ├── 3babfde10935946417c20655960c423b6e89ccd8.nq.gz
│   ├── 3c348389eaf56c9c743ad7755bb115a87c19ba68.nq.gz
│   ├── 3d1ca8270f783e136940325b636b7915496c57f8.nq.gz
│   ├── 40bfe2fa6a67b2cc686467eb131fcdf8a0b07cf8.nq.gz
│   ├── 50f590cf0454239105493242c6c0a8a77ad00edc.nq.gz
│   ├── 5d04cf0688db3bde1769b703dc5100d35faebe73.nq.gz
│   ├── 60c51d93c0c81bc8c82d13d377c0e1b4fe58c471.nq.gz
│   ├── 610f8057af421224d81b03adc2de89c9d295850e.nq.gz
│   ├── 779559c54f0b8f2e856681ec70a3833189739753.nq.gz
│   ├── 78981922613b2afb6025042ff6bd878ac1994e85.nq.gz
│   ├── 7cb3b0e101840b22bf620e4b15f46c733054e8e2.nq.gz
│   ├── 86b9b470efe80a9c8c0b4142e11c090284e1d8d6.nq.gz
│   ├── 871066d831a5657f09f5b808741f2512c4d3eba5.nq.gz
│   ├── 8c8d883a27f7b32f48c6c551da323d8885416d24.nq.gz
│   ├── 8ea8db4dac10cd1b688d1fc47f20465ab4a86a0c.nq.gz
│   ├── 931847ea86960f74fa9970c1184f8ea5ba5119bf.nq.gz
│   ├── 935cdbafb323ac615fc22c86cfbaf3f2359771b8.nq.gz
│   ├── 93cb80921e21aed8acfdd81bf5c096138f2e228f.nq.gz
│   ├── 9abf3f797da2acc3d75efe3a8f14fb6125391e87.nq.gz
│   ├── 9eb3f0b91efca8b2091b132e4fe8b16c0468c526.nq.gz
│   ├── a717ddc7d0545dcfceee783ef6dde5442bb886a1.nq.gz
│   ├── a940ceadbb079bf7c80360c35b25bbbb9d5aa699.nq.gz
│   ├── ac2e4549c7d7acf2d1c5b620258f021d6636ea5b.nq.gz
│   ├── b7b5e6d653b94ab9c6dbb08d45d464c27545a389.nq.gz
│   ├── d64c4ca28695d25478719cb14bf4689f39f75b64.nq.gz
│   ├── da2078a62efd6a47d9ce3e6c70cab55ad262479c.nq.gz
│   ├── de5b728a028324e9158e82588e415e64a3b2a794.nq.gz
│   ├── e256a314d7da6a2f3ac28de93938f0d4f6b40b77.nq.gz
│   └── e305767ef750e880c38c7185e5c8e4d76c5e2ade.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── c3a75242772a5026a49c4017a16d9b3543b62776.nq.gz
├── filetree
│   └── c3a75242772a5026a49c4017a16d9b3543b62776.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 49 files
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

[json5/json5](https://github.com/json5/json5)

---
*Parsed on 2026-09-16 by [repolex](https://repolex.ai)*
