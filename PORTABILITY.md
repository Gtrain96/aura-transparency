# Portability — The Creator's Reserved License (§6)

> Plain-English explanation of [§6 of the License](./LICENSE#6-creators-portability-right).
> The License text is the binding instrument; this document is for orientation.

## The short version

When the Creator (Ian Gilbert) commits source code, system instructions,
configuration schemas, evaluation harnesses, design tokens, or any other
work-of-authorship to this repository under the Aura Ethics License v1.0,
**and** certifies that no Confidential Data is included in that commit, the
Creator retains a perpetual, irrevocable license to use, modify, and
redistribute those works through any future project of any future employer.

This means the Creator can:

- Take work in this repo to a new employer and continue to use, modify, and
  build on it
- Publish that work in another public repository under any compatible license
- Incorporate it into commercial products, provided they comply with §4
  (Ethics Addendum) and §7 (Data Segregation)
- Sublicense it to others on any terms consistent with this License

This right is **not** affected by:

- Any employment agreement, work-for-hire, or assignment the Creator has
  signed or may sign
- Transfer of this repository to another organization (e.g., to Innovest)
- Termination of the Creator's rights under any other agreement
- Termination of any third party's rights under this License

## What is NOT covered by §6

The Creator's portability right does not extend to:

1. **Confidential Data** (§7) — client identifiers, account data, portfolio
   holdings, proprietary CMA inputs, PII, or anything classified Confidential
   under any employer's information security policy. These remain the
   property of the lawful possessor and were never licensed to begin with.

2. **Other contributors' work** — code or content authored by others and
   contributed under separate terms. Those contributors hold their own
   rights; the Creator's §6 right is limited to the Creator's own
   authorship.

3. **Trademarks and trade names** — "Innovest," "Project Aura," "Aurora,"
   or any other organizational mark. Trademarks are licensed separately
   from copyright and are not granted under this License.

## Why §6 exists

The Creator developed the Aura platform's deterministic-first architecture
— HITL classification, RLS partitioning, truth-table-as-IaC, the persona-
driven design — through extensive personal study, planning, and authorship.
Much of that intellectual capital lives in code, configs, and documentation
that have been refined into the patterns this repository publishes.

§6 ensures that the Creator's career mobility is not constrained by the
specific organizational arrangements under which any individual version of
that work was first written. The Creator's intellectual capital travels
with the Creator; the Creator's employer's confidential data does not.

This is the standard arrangement in academic publishing (the author
retains a license to use their own published work in subsequent research)
and in patent law (an inventor retains rights distinct from any assignment
of a specific patent). §6 applies the same principle to source code and
methodology in a fiduciary context.

## How the certification under §6(b) works

When the Creator commits to this repository, the commit itself constitutes
a certification under §6(b) that the contents of that commit contain no
Confidential Data, subject to the Creator's good-faith review at the time
of commit.

If a commit later turns out to have inadvertently included Confidential
Data (e.g., a debug log was checked in by mistake), the appropriate remedy
is:

1. Remove the offending content via a follow-up commit (and, if necessary,
   a force-push or repository rewrite coordinated with the affected party)
2. The §6 right does not extend to the inadvertently-included Confidential
   Data
3. The §6 right does extend to the surrounding work-of-authorship that
   would have been certifiable absent the inadvertent inclusion

The right is robust to honest mistakes; it does not legitimize deliberate
inclusion of Confidential Data.

## Examples

**Example 1 — Code mobility.** The Creator writes a Python module
implementing the truth-table-as-IaC contract for the Aura platform.
The Creator commits it to this repository under AEL v1.0, with no
Confidential Data included. Three years later, the Creator moves to a
different RIA. The Creator may incorporate the truth-table-as-IaC module
into the new RIA's platform, modify it, and continue to develop it. The
new RIA's deployment must comply with §4 (Ethics Addendum) — the
substantive obligations travel with the code.

**Example 2 — Masked data.** During the Creator's tenure at Innovest,
the platform processes anonymized RFP responses. The Creator commits the
anonymization script and the resulting synthetic-test corpus to this
repository, certifying no Confidential Data is included. The Creator may
use both the script and the synthetic corpus in any future project. The
underlying client identities, never published, are not licensed and
remain Innovest's. Note: §7 specifically clarifies that masking is a
*privacy control, not a license grant* — you cannot mask Confidential
Data and thereby acquire rights to it. The synthetic corpus is
license-portable because it is synthetic, not because it was masked from
something that wasn't.

**Example 3 — Repository transfer.** When `Gtrain96/aura-transparency` is
transferred to `Innovest/aura-transparency`, the §6 right is not affected.
The Creator retains the license to all Creator-authored contributions
made before the transfer, and the transfer itself does not constitute a
new assignment of those rights.

## Practical guidance for the Creator

To make §6 maximally enforceable in future situations:

1. **Keep certification meaningful.** Don't commit data you wouldn't be
   comfortable defending as non-Confidential at deposition. If unsure,
   don't commit.
2. **Maintain provenance of authorship.** When the Creator authors a
   piece of work, the git history is the record. When others contribute,
   their commits should be signed under their own attribution so the
   §6 right correctly identifies what the Creator authored.
3. **Document the boundary.** Where Creator-authored work integrates with
   employer-confidential systems, the boundary should be visible in the
   architecture (e.g., a stable interface where one side is public and
   one side is private). This makes the §6 carve-out unambiguous.
4. **Treat repository transfer as preserving, not extinguishing.** If
   this repository is transferred (e.g., to Innovest), reaffirm §6
   coverage in the transfer documentation. The License says the right
   survives transfer; the documentation should not contradict that.

## Practical guidance for employers and successor owners

§6 is structured to be respected by good-faith counterparties:

- The Creator's right does not allow extraction of any Confidential Data.
- The Creator's right does not allow use of organizational trademarks.
- The Creator's right does not interfere with the employer's continued
  use of the same code through the License's primary grants (§2 and §3).
- The Creator's right is non-exclusive — the employer's use is not
  diminished by the Creator's parallel use.

The intent is a clean parallel: the Creator and the employer (or any
successor) both retain rights to use the licensed code, each subject to
the same §4 ethics obligations, neither dependent on the other's
permission.
