# SCANOSS dataset samples

Data retrieved 6 November 2026

SCANOSS is a software company based in Madrid. It provides data and tools that show what is inside software: the open source it contains, the licences that apply, known vulnerabilities and the cryptography it uses.

This repository holds one small sample from each of three SCANOSS datasets. Each sample covers one open source package at one version.

Every file here is real, unedited output from the SCANOSS API. We have not changed, removed or added any results.

## The samples

- [License](license/): licence evidence for Redis 7.2.4. It shows which licences SCANOSS found in each file of the package.
- [Security](security/): known vulnerabilities for Apache Log4j Core 2.14.1. This is the version affected by Log4Shell.
- [Encryption](encryption/): cryptography findings for Bouncy Castle 1.78.1. It shows where each algorithm is used in the code.

## What is in each folder

Each folder has the raw API reply as a JSON file and the same data as a CSV file. The README in each folder says what was scanned and what each column means.

## More information

You can learn more about SCANOSS and its datasets at [scanoss.com](https://scanoss.com). The API documentation is at [docs.scanoss.com](https://docs.scanoss.com).
