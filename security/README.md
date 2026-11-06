# SCANOSS security sample: Log4j 2.14.1

Data retrieved 6 November 2026

This is real, unedited output from the SCANOSS API.
We have not changed, removed or added any results.
Includes every record the API returns, including vendor advisories for their own patched builds.

## What was scanned

- Package: Apache Log4j Core (`pkg:maven/org.apache.logging.log4j/log4j-core`)
- Version: 2.14.1, the last version before the Log4Shell fix
- Question asked: which known vulnerabilities affect this version?
- Command: `scanoss-cli vulnerabilities --purl 'pkg:maven/org.apache.logging.log4j/log4j-core' --requirement '2.14.1'`

SCANOSS returned 9 records. They include Log4Shell (CVE-2021-44228) and the follow-up flaws found in December 2021.

## Files

- `log4j-core-2.14.1-vulnerabilities.json`: the full API reply.
- `log4j-core-2.14.1-vulnerabilities.csv`: the same data as a table. One row per record.

## Columns in the CSV

| Column | Meaning |
|---|---|
| `id` | The advisory ID. `GHSA-…` is a GitHub advisory. `RHLW-…` is a Red Hat Lightwell advisory. |
| `cve` | The CVE ID, if there is one. |
| `source` | Where SCANOSS got the record. OSV is the Open Source Vulnerabilities database. |
| `severity` | How serious the flaw is: CRITICAL, HIGH, MODERATE or LOW. Empty if the source gives none. |
| `cvss_vector` | The CVSS vector, which describes how the flaw can be exploited. |
| `cvss_score` | The CVSS score as returned by the API. |
| `epss_probability` | EPSS: the chance of this flaw being exploited in the next 30 days, from 0 to 1. |
| `epss_percentile` | How this EPSS score ranks against all CVEs, from 0 to 1. |
| `published` | When the record was first published. |
| `modified` | When the record last changed. |
| `fixed_versions` | Versions that fix the flaw. There can be one per release line. |
| `summary` | A short description. |

## More information

https://docs.scanoss.com
