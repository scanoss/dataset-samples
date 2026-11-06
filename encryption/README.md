# SCANOSS encryption sample: Bouncy Castle 1.78.1

Data retrieved 6 November 2026

The mined_at date shows when SCANOSS analysed this version of Bouncy Castle. Data retrieved shows when we pulled the results from the API.

This is real, unedited output from the SCANOSS API.
We have not changed, removed or added any results.

## What was scanned

- Package: Bouncy Castle for Java (`pkg:maven/org.bouncycastle/bcprov-jdk18on`)
- Version: 1.78.1
- Question asked: where in the code is cryptography used, and which algorithms?
- API call: `POST https://api.scanoss.com/v3/cryptography/reachability/component` with only the package and version. This returns the stored crypto findings for that version.

SCANOSS returned 2,172 findings in 425 files.
They range from AES and SHA-256 to post-quantum algorithms such as SPHINCS+ and Dilithium.

## Files

- `bouncycastle-1.78.1-crypto-findings.json`: the full API reply.
- `bouncycastle-1.78.1-crypto-findings.csv`: the same findings as a table. One row per finding.

## Columns in the CSV

| Column | Meaning |
|---|---|
| `version` | The version scanned. |
| `file` | The source file the finding is in. |
| `start_line`, `end_line` | The lines in that file. |
| `asset_type` | What was found: an algorithm, a certificate, or related material such as a key or salt. |
| `algorithm` | The algorithm name, such as AES or SHA-256. Empty for some asset types. |
| `algorithm_family` | The wider family, such as AES or SHA-2. |
| `primitive` | The kind of crypto: block cipher, hash, signature, key agreement and so on. |
| `operation` | What the code does with it, such as encrypt or sign. |
| `oid` | The standard object identifier for the algorithm, if known. |
| `api` | The Java class or method used. |
| `match` | The code that was matched. For some findings this is a method name, not a line of code. |
| `source` | `direct` means the code is in this package itself. |
| `rules` | The detection rules that fired. |
| `finding_id` | SCANOSS's ID for the finding. |

## More information

https://docs.scanoss.com
