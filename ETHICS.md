# Ethics — Plain-English Summary

> Human-readable summary of [§4 (Ethics Addendum), §5 (Tamper-Evident Receipts),
> and §9 (Public Audit Right) of the License](./LICENSE). The License text is
> the binding instrument; this document is for orientation only.

## TL;DR

If you use the Aura platform — as a developer, operator, or end-user — you
agree to five things:

1. **A qualified human is in the loop.** Any fiduciary-touching system using
   the Work runs under a CFA charterholder or equivalent professional.
2. **You tell the client.** Any output reaching a client discloses that an
   AI-assisted process produced it (form and granularity may vary by
   audience — see below).
3. **You don't strip the gates.** The deterministic provenance gates
   (HITL classification, RLS partitioning, source pointer hashes,
   truth-table validation) stay in force.
4. **You don't deceive.** No "vibes-marketing" the system as something other
   than what it is.
5. **You answer when audited.** Anyone can request your system instructions,
   gate rules, and benchmark scores. You answer within 30 days.

## Why these conditions exist

Conversational LLM systems are general-purpose tools. Used without
constraints, they can produce confident, fluent, plausible output that is
wrong. In a fiduciary context — retirement plans, family wealth, foundation
endowments — that's not a quality problem, it's a duty-of-care problem.

The CFA Institute Code of Ethics and Standards of Professional Conduct
(I through VII) sets the floor. The Aura platform is built to meet that
floor by design: the deterministic gates are how we know an answer
*can be* defended, not just *sounds* defensible.

This License binds developers and users to keep those gates in force. If
you strip them — even with good intentions — you've created something that
no longer carries the audit story it was designed to carry.

## The five obligations in detail

### §4.1 — Supervision

A CFA charterholder or equivalent fiduciary professional supervises any
Fiduciary System deployment. "Supervision" means active, contemporaneous
oversight — not a name on a compliance attestation filed annually.

If your jurisdiction does not recognize the CFA charter, an equivalent
licensed professional (e.g., registered investment adviser, ERISA fiduciary
counsel, equivalent in non-US jurisdictions) satisfies this obligation.

### §4.2 — Disclosure (with audience tiers)

The hard requirement: anyone receiving output produced with this Work knows
that an AI-assisted process produced it.

The flexibility: the **form and granularity** of disclosure varies by
audience. This is intentional, and reflects the operator's reality:

**External audiences (clients, prospects, regulators-in-routine-contact):**
A statement that the response was produced through a reviewed,
AI-assisted process operating under CFA-aligned controls satisfies §4.2.
You are not required to disclose internal model identifiers, prompt text,
or implementation details to external recipients. You ARE required to make
clear that automated systems materially shaped the response.

**Internal audiences (qualified reviewers, auditors, regulators in an
examination, anyone exercising the §9 Public Audit Right):**
Disclosure is more granular. You must be able to produce the Provenance
Gates' decision records sufficient to reconstruct how the output was
produced.

This split — ambiguous-but-honest externally, transparent internally — is
how the License accommodates real client communications without creating
either deception or operational impossibility.

### §4.3 — Provenance Preservation

The Provenance Gates are:

| Gate | What it does |
|---|---|
| **HITL Classification** | Analyst confirms partition labels at intake. Label is deterministic from that point on. |
| **RLS Partitioning** | Database physically cannot return cross-partition rows. |
| **Source Pointer Hashes** | Every numeric claim carries a hash that re-validates against the source on retrieval. |
| **Truth-Table Validation** | Unsourced numerics fail-closed and route to human review. |
| **Fail-Closed Routing** | When a gate fails, the system never silently degrades — output is blocked, not approximated. |

You can replace these with functionally equivalent gates that meet the
same audit standard. You cannot strip them.

### §4.4 — No Deception

No marketing the system as a "human-only" process. No prompt-engineering
to evade disclosure obligations. No representing automated output as
hand-authored when it isn't.

This is the floor below which CFA Standards V(B) and V(C) are violated as
a matter of professional conduct regardless of what the License says.

### §4.5 — CFA Standard VII Compliance

If you hold the charter, you comply with Standard VII when you use the
Work — regardless of any contrary direction from your employer. The
License gives Standard VII teeth that the employer cannot override.

## Faith-stance neutrality (§4.6)

The Work supports Catholic-USCCB, Christian-Evangelical-BRI, denominational,
and secular partitions. The License is neutral as to which one any operator
chooses for which client.

What is NOT permitted: using the Work to ridicule, attack, or systematically
disadvantage any faith community whose screening criteria are supported by
the Work's partitioning system. The faith-partition design exists to serve
those communities; weaponizing it against them is a breach of §4.6.

## Tamper-Evident Receipts (§5)

Every output going to a third party carries (or is accompanied on request
by) a receipt with:

- Source pointer hashes for all numeric claims
- The RLS partition identifier in effect during retrieval
- Decision records of all gates that fired
- The version of the Work used

You can use your own receipt format. The substance — the audit substance —
is what's required.

## Public Audit Right (§9)

Any person — client, regulator, journalist, academic — can write and ask:

- What version of the Work are you running?
- What system instructions are configured?
- What's in your gate rule packs?
- What were the last eval-cycle benchmark scores?

You answer within 30 days. You can redact Confidential Data, illegal-to-
disclose information, and security-compromising details, but you have to
identify what you redacted.

This is CFA Standard III(D) (Performance Presentation) applied to
methodology, not just performance.

## What this means for the platform's clients

If a client of an Aura platform operator asks "did AI write this?" — the
honest answer is yes, an AI-assisted process produced it, reviewed by a
qualified human. Operators are free to phrase this in their own voice.
What they are not free to do is deny it.

That's the moat. Vibes-coded chat tools cannot make this commitment without
also undertaking the supervision, gate-preservation, and audit obligations.
The Aura platform makes the commitment binding from day one.
