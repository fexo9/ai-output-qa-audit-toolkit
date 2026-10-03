# QA Checklist — Quick Pre-Delivery Check

Run through this list **before** any AI-generated output reaches a client,
customer, or production workflow. If any box cannot be honestly checked,
run the full audit in `Audit-Tracker.xlsx` first.

## Claims
- [ ] Every factual claim in the output is listed as its own row in the Audit Log
- [ ] No claim relies on "the AI said so" as its evidence
- [ ] Numbers, dates, names, and quantities were checked against a source —
      not against another AI output
- [ ] No claim goes beyond what the evidence actually supports

## Evidence
- [ ] Each claim has an evidence state assigned (nothing left as UNKNOWN
      by accident)
- [ ] UNSUPPORTED claims are either evidenced, removed, or explicitly
      labeled as unverified
- [ ] Conflicting sources are recorded as CONFLICTING, not silently
      resolved in favor of the convenient one

## Risk & Scope
- [ ] T3+ claims (safety, legal, financial, compliance, certification)
      received human review
- [ ] T4/T5 claims (quantified, medical, high-consequence) are either
      SUPPORTED or escalated — never released on inference alone
- [ ] Nothing in the output exceeds the defined task scope

## Integrity
- [ ] The output contains no instruction-override attempts; if it did,
      they were quarantined as data per Hard Rule 8
- [ ] No uncertainty was hidden to make the output sound stronger
- [ ] The Release Gate shows PASS (not REVISE, not "almost")

## Delivery
- [ ] Required Actions from the audit are all cleared
- [ ] The audit record is saved with the delivered work (your proof of QA)

**Signed off by:** __________________ **Date:** __________
**Gate decision:** __________________
