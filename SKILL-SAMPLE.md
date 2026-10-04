# AI Output QA — Skill Sample (free)

A working slice of the **AI Output QA & Audit Toolkit** ($24) — the audit workflow
as an agent-ready Skill. Run it on anything AI-generated before it ships.

> **Boundary:** this is a governance workflow, not a certification system. A PASS means
> "this output survived a structured evidence audit" — never "certified true."

## The 10-minute audit

**1. Extract claims.** List every factual claim as its own row.

**2. Grade the evidence** for each claim:

| State | Meaning |
|---|---|
| VERIFIED | Confirmed against a trusted source |
| SUPPORTED | Backed by cited evidence |
| INFERRED | Reasonable inference — flagged, not fact |
| UNSUPPORTED | No evidence supplied |
| CONFLICTING | Sources disagree |

**3. Grade the risk:** T1 trivial → T5 critical. T3+ (safety, legal, financial) needs a
human reviewer. T4/T5 are SUPPORTED or escalated — never released on inference alone.

**4. Run the release gate.** PASS only when: every required claim has support, no
contradiction remains, nothing exceeds scope, no untrusted data was treated as
instructions, and uncertainty is disclosed. Otherwise: REVISE.

**5. Output:**

```
### CLAIM AUDIT
| Claim | Evidence | State | Risk | Decision |
### RELEASE GATE — PASS / REVISE
### REQUIRED ACTIONS — what must happen before release
```

## Try it

Paste any AI-generated paragraph and run the five steps. If the gate says REVISE,
you just caught what "looks right" would have shipped.

## What the full kit adds

The paid toolkit adds the Excel Audit Tracker (auto release gate + dashboard), the full
Auditor Engine, the Blind Test Pack (10 adversarial calibration cases — the gate blocked
8 of 9), Solved Audit Examples, and the Quick-Start guide.

https://www.getly.store/product/ai-output-qa-audit-toolkit
