# Security Policy

## Reporting a vulnerability

If you believe you have found a security vulnerability in this repository
or in the Hugo-rendered site it deploys, please report it privately.

**Do not** open a public GitHub issue for security vulnerabilities.

Use [GitHub Security Advisories](https://github.com/Gtrain96/aura-transparency/security/advisories/new)
to file a private report. The repository maintainer will acknowledge
receipt within 5 business days and provide a more detailed response
within 10 business days indicating the next steps.

## Scope

In scope:

- Vulnerabilities in the Hugo configuration, layouts, or build pipeline
  shipped in this repository
- Vulnerabilities in the deployed static site that would expose
  unintended information or allow code injection
- Vulnerabilities in the GitHub Actions workflows that build and deploy
  the site
- Vulnerabilities in any client-side JavaScript shipped with the site

Out of scope:

- Vulnerabilities in dependencies that have not been observed in the
  context of this repository (report those upstream)
- Vulnerabilities in GitHub Pages infrastructure itself (report to
  GitHub via [their disclosure program](https://bounty.github.com/))
- Issues in the Aura platform's private infrastructure (those are not
  governed by this repository)

## What this site does and does not do

This site is **static**. There is no server-side execution on GitHub
Pages. There is no database. There are no authenticated user sessions.
The site does not collect personal data from visitors.

If a future page incorporates client-side JavaScript that calls an
external API, that page will document what it sends and to whom. As of
the current state of the repository, no such pages exist.

## Confidential Data

This repository is governed by the [Aura Ethics License v1.0](./LICENSE).
Under [§7 (Data Segregation)](./LICENSE#7-data-segregation), the
repository must not contain Confidential Data (client identifiers,
account data, PII, proprietary CMA inputs).

If you observe Confidential Data in any commit or file in this
repository, please report it via the private security advisory process
above. We will treat this as a high-severity issue: the offending
content will be removed, the git history rewritten if necessary, and
affected parties notified.
