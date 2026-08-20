# Hridoy Samadder — Forensic Audit & Evidence Package
### Read-only forensic reconciliation · evidence cutoff **2026-08-20 (~21:29 UTC)** · compiled 2026-08-21 (Asia/Dhaka)

All figures below are bound to the cutoff. The audit was **strictly read-only** — no repository, database, deployment, or DNS state was modified while producing any of this (verified: zero commits, clean working trees across every inspected repo).

---

## Files

| File | What it is |
|---|---|
| **[`HRIDOY_FORENSIC_AUDIT_2026-08-20.md`](./HRIDOY_FORENSIC_AUDIT_2026-08-20.md)** | **The main document** — the current 21-section forensic audit, bilingual (English + *সহজ বাংলায়*), same structure as the original 2026-08-07 audit but primary-verified this pass. |
| [`HRIDOY_FORENSIC_AUDIT_2026-08-20.html`](./HRIDOY_FORENSIC_AUDIT_2026-08-20.html) | The exact same 21-section audit as a self-contained web page (sticky table of contents, light/dark toggle, Print → Save-as-PDF). |
| [`HRIDOY_FORENSIC_RECONCILIATION.md`](./HRIDOY_FORENSIC_RECONCILIATION.md) | The long-form 32-section reconciliation — source-weight audit, model self-audit, execution-state audit, AI-collaboration record, PR enumeration, full 22-repo sweep. The deepest supporting record. |
| [`dossier.html`](./dossier.html) | The polished visual "Evidence Dossier" — the one-glance canonical (KPIs, systems, capabilities, truth table). |
| [`evolution.html`](./evolution.html) | Day-by-day build & decision evolution — systems × weeks heatmap, SHA-bound timeline, decision-evolution, failure→response, metrics. |
| [`card.html`](./card.html) | One-page profile card (print/PDF-ready). |

*(HTML files are self-contained: open in any browser; fonts load online and fall back gracefully offline.)*

---

## Headline — evidence-bound

- **22 repositories** inspected read-only — all contain real content, none empty.
- **386 merged pull requests** of 396 total (enumerated via GitHub search, **not** inferred from the highest PR number).
- **2 / 2** machine-attested CI suites **green on the first run** (GitHub Actions runs `31182879628`, `31185419765`).
- **34,244-medicine** catalogue + 90,258 preserved import-source rows (SQLite-counted).
- **OushodhOS production-live**; verified DB backup + restore (CI run `32173119387`); `/api/health` commit-SHA proof; boot-guard.
- **Evidence-governance as named code modules** across repositories built weeks apart (`snigdha_approval_gate.py`, `oyshe_self_eval.py`, decision logs, audit logs).
- **Solo — confirmed** (the "Choton" identity is the builder himself).

## Not established (stated plainly, not as deficiencies)

Internet-scale load · multi-year longevity · team leadership · independent security certification. The Mumbai→Singapore DB migration was committed but **not yet run** at the cutoff. **"World-class"** is a reader's reaction to the work, not a self-claim — there is no population benchmark that makes it a fact.

---

*Method: claim strength never exceeds evidence strength, and evidence strength is never deflated by reflexive caution. Every load-bearing claim is traced to a primary source (code, git/CI, SQLite, PR state) and tagged by provenance. A later repository state may supersede this snapshot without making it wrong — it is a dated, reproducible reconstruction.*
