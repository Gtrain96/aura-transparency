# Aura Transparency

> Public methodology, system instructions, and ethics for the Aura sell-side
> RFP and buy-side manager-DD platform.

**License:** [Aura Ethics License v1.0 (DRAFT v0.1)](./LICENSE) — Source-Available · Ethics-Restricted · pending counsel review

**Live site:** *(GitHub Pages deploy pending — Hugo content migration in flight)*

---

## What this repository is

This repository publishes the parts of the Aura platform that are intended to
be auditable by clients, regulators, and the CFA Institute community:

- **System instructions** for each persona (Retirement · Wealth · Foundation & Endowment)
- **CFA Code of Ethics alignment** mapping each system control to a CFA Standard
- **Provenance methodology** — HITL classification, RLS partitioning, truth-table
  validation, fail-closed gates
- **Benchmark methodology** — the single algorithm + eval harness against which
  every release is measured
- **Software engineering principles** — Karpathy-inspired disciplines applied to
  fiduciary-context coding

It does NOT publish: client data, account holdings, proprietary CMA inputs,
PII, or any data classified Confidential under [§7 of the License](./LICENSE).
Those remain on the operator's infrastructure.

## What this repository is NOT

- Not an OSI-approved open source license. It is **Source-Available with
  binding ethics conditions**.
- Not a substitute for fiduciary advice. The platform's language-model
  components are not suitable, in isolation, for the discharge of fiduciary
  duties. See the [Disclaimer of Warranty](./LICENSE#11-disclaimer-of-warranty).
- Not a complete reproduction of the platform. Confidential code, client
  data, and proprietary CMA logic remain on the operator's infrastructure.

## Why publish this at all

CFA Standard III(D) (Performance Presentation) and Standard V(B)
(Communication with Clients) put a burden on practitioners to disclose method.
Modern AI-assisted systems often fail this standard by being opaque "black
boxes." This repository is the operator's commitment that everything
load-bearing in their methodology — gates, system instructions, partition
rules, benchmark scores — is publicly inspectable by any party who asks.

The [Public Audit Right (§9)](./LICENSE#9-public-audit-right) makes this
binding for any party that licenses the platform.

## Key documents

| File | Purpose |
|---|---|
| [LICENSE](./LICENSE) | Aura Ethics License v1.0 — the binding terms |
| [ETHICS.md](./ETHICS.md) | Human-readable summary of the Ethics Addendum (§4) |
| [PORTABILITY.md](./PORTABILITY.md) | The Creator's reserved license rights (§6), explained |
| [CONTRIBUTING.md](./CONTRIBUTING.md) | How to contribute; DCO sign-off; ethics gates |
| [SECURITY.md](./SECURITY.md) | Vulnerability disclosure |

Once the Hugo content migration is complete, the rendered site will publish:

- `/standards-ethics/` — CFA alignment, LLM limitations, audit trail policy
- `/methodology/` — HITL classification, truth-table-as-IaC, RLS partitioning, fail-closed gates
- `/thought-leadership/` — agentic engineering, AI ecosystem essays
- `/changelog/` — versioned disclosure of system-instruction and gate changes

## Status

| Item | State |
|---|---|
| License (AEL v1.0) | **Draft v0.1** · pending counsel review |
| Hugo content migration from main repo | In flight |
| GitHub Pages deploy workflow | Pending Hugo content |
| Mirror-from-main automation | Pending |

## Repository ownership

Currently owned by [@Gtrain96](https://github.com/Gtrain96). On the schedule
agreed with Innovest, transfer to `Innovest/aura-transparency` is anticipated.
Per [§6 of the License](./LICENSE#6-creators-portability-right), the
Creator's reserved license is unaffected by repository transfer.
