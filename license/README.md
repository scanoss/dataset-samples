# SCANOSS licence sample: Redis 7.2.4

Data retrieved 6 November 2026

This is real, unedited output from the SCANOSS API.
We have not changed, removed or added any results.
Includes licences found in bundled third-party files, not only Redis's own licence.
Automated detection can mislabel a few bundled files. For example, linenoise is BSD-2-Clause, not BSD-3-Clause.

## What was scanned

- Package: Redis (`pkg:github/redis/redis`)
- Version: 7.2.4
- Question asked: which licences appear in each file of this version?
- Command: `scanoss-cli licenses evidence --purl 'pkg:github/redis/redis' --requirement '7.2.4'`

SCANOSS found licence evidence in 304 files. Most are BSD-3-Clause, which is the Redis licence.
Bundled libraries show their own licences, such as MIT for Lua.

## Files

- `redis-7.2.4-license-evidence.json`: the full API reply.
- `redis-7.2.4-license-evidence.csv`: the same data as a table. One row per licence found in a file.

## Columns in the CSV

| Column | Meaning |
|---|---|
| `purl` | The package scanned. |
| `version` | The version scanned. |
| `file` | The file the licence was found in. |
| `licence` | The licence, as an SPDX ID. |
| `source` | Where in the file it was found. `header_declared`: a comment at the top of a file. `notice_declared`: a licence or notice file. `metadata_declared`: build or package metadata. |
| `confidence` | How sure the detector is, from 0 to 1. |
| `detector` | The tool that found it. |
| `evidence_start`, `evidence_end` | Where the matched text sits in the file, counted in bytes from the start. |
| `evidence_url` | A link to the matched text on the SCANOSS API. You need an API key to open it. |

## More information

https://docs.scanoss.com
