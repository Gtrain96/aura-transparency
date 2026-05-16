# Contributing

Thanks for your interest in contributing to Aura Transparency.

## License of contributions

By submitting a pull request to this repository, you agree that your
contribution will be licensed under the [Aura Ethics License v1.0](./LICENSE).
The License includes binding ethics conditions (§4) and a Public Audit
Right (§9). Please read the License before contributing.

## DCO sign-off required

All contributions must be signed off under the [Developer Certificate of
Origin](https://developercertificate.org/) by including a line of the form:

```
Signed-off-by: Your Name <your.email@example.com>
```

at the bottom of each commit message. Use `git commit -s` to add this
automatically.

By signing off, you certify that:

- You have the right to submit the contribution under the License;
- The contribution is your original work, or contains other-licensed work
  that you have appropriately attributed; and
- The contribution does not include Confidential Data as defined in
  [§7 of the License](./LICENSE#7-data-segregation).

## What to contribute

The following kinds of contribution are welcome:

- **System instructions** for new personas or partition variants
- **Provenance methodology** improvements — new gate designs, audit-trail
  formats, receipt schemas
- **Benchmark methodology** improvements — new metrics, new eval-harness
  patterns, new reference corpora (synthetic only)
- **CFA-alignment documentation** — clarifications, additional standards
  mappings, updated Code references
- **Thought-leadership essays** under `content/thought-leadership/`
- **Bug fixes** in Hugo templates, layouts, build scripts

The following are NOT welcome and will be rejected:

- Any client data, account holdings, or PII
- Any proprietary CMA inputs or third-party-licensed data without proof
  of redistribution rights
- Anything that would strip or weaken the Provenance Gates documented in
  the methodology

## Review process

Pull requests are reviewed against:

1. **Substance.** Does the contribution improve the methodology or its
   documentation?
2. **License compliance.** Is the contribution clean of Confidential Data?
   Does it preserve ethics obligations?
3. **Audit-trail.** Does the contribution maintain the public-auditability
   commitment (§9)?

## Reporting issues

Use GitHub Issues for documentation gaps, broken links, or questions
about the methodology. For security issues, see [SECURITY.md](./SECURITY.md).

For questions about the License itself, open a discussion — substantive
License clarifications may be incorporated into a future version.
