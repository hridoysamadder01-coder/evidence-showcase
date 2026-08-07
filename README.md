# HRIDOY SAMADDER — Evidence-Mapped Capability Showcase

**Solo builder · Bangladesh · AI-leveraged (no team, no institutional backing)**
Contact: hridoysamadder01@gmail.com · GitHub: `hridoysamadder01-coder`

> **How to read this document.** Every claim carries a tag: **[FACT]** = verified against artifacts (git history, files, or GitHub-machine CI runs; provenance noted), **[INFERENCE]** = labeled interpretation, **[UNKNOWN]** = honestly untested, **[BUILDER-STATED]** = the builder's own account, with supporting artifacts noted. Compiled from a zero-write forensic audit of all 16 repositories (2026-08-07); the full 21-section audit report, with commit SHAs and file paths for every claim, is available on request. Nothing here was created for show — every referenced test, ledger, and measurement existed in the repositories before this document.

---

## 1. Headline facts

- **16 repositories, ~1,591 commits, built in ~8.5 weeks** (2026-06-08 → 2026-08-05). **[FACT — git history, all repos]**
- **All human commits resolve to one person** — three author identities share one email across repos. Solo, verified, not claimed. **[FACT — git author-email analysis]**
- **AI used as leverage, openly:** ~746 commits authored by AI sessions, ~845 under the builder's own identities; the division is visible in the history, not hidden. **[FACT — git shortlog]**
- **4 systems actually deployed** (pharmacy SaaS beta, voice-AI mission control + public API, AI tutor, stock-market terminal — all on Render). **[FACT — deploy configs + repo-documented live URLs]**
- **Machine-attested test suites as of 2026-08-07:** pharmacy SaaS — 342 backend tests + 13 frontend suites + production build, **green on GitHub's machines, first run** (Actions run 31182879628); voice-AI system — 106+28+38+12 harness checks, 45 backend unit tests, typecheck/lint/build, **green first run** (run 31185419765). **[FACT — GitHub Actions, machine-verified]**
- **Day-to-day operation runs from a mobile phone via tunnel links** — per the builder's own account; the repositories contain artifacts built specifically for that workflow (an auto-learning tunnel-address module, phone-path launcher scripts, phone-side verification notes in the ledgers). Not machine-verified. **[BUILDER-STATED — artifact-supported]**

## 2. What was built (main systems)

| System | What it is | Evidence class |
|---|---|---|
| **OushodhOS** | Bangla-first pharmacy POS/inventory SaaS: camera medicine recognition (Gemini vision + on-device local-first catalog), invoice OCR with arithmetic-verified self-heal, multi-tenant isolation live in production, Android APK, thermal printing | [FACT — 582 commits, 111 merged PRs, 37-table schema, CI-green suites] |
| **HS-OS / HRIDOY** | Voice-first "mission control" AI: hand-rolled Gemini Live client (zero AI-SDK dependencies), local voice-clone of the builder's own voice on his own GPU (cost ৳0, offline-capable), speaker-similarity gating, mood-routed TTS, deployed public text API | [FACT — 434 commits; package.json runtime deps = react/react-dom only; voice pipeline repo-documented] |
| **masterdatabase** | 34,244-medicine Bangladesh master catalog with five-field SHA-256 identity ("never match by brand alone"), human photo-verification pipeline with 178 recorded verdicts — including rejections and a caught 1000× mcg/mg source-data error | [FACT — schema CHECKs + runtime guards + committed review ledgers] |
| **EduVerse AI** | Bangla AI tutor (RAG + MCQ) with real `usageMetadata` token accounting and a measured-vs-estimated provenance flag on every cost figure | [FACT — code; deployed] |
| **TechStock-OS** | Electronics-shop POS: on-device ML Kit OCR per sale, Gemini vision once per product (cost discipline), APK built by real CI with a verifiable bot-commit trace | [FACT — 184 tests + CI artifacts in-tree] |
| **DSE-AI-TRADER** | Dhaka Stock Exchange terminal that is deliberately LLM-free — in-code disclaimer: every generated sentence cites a measured value | [FACT — code] |

## 3. Demonstrated capabilities (each with evidence)

- **Evidence-governed engineering.** Append-only decision log (D1–D71) with founder quotes and supersession chains; 195-entry audit log; a verification ledger that binds human sign-offs to build hashes so verdicts *expire* on new deploys; a measured sycophancy index fed back into the AI's own prompt. **[FACT — files in HS-OS]**
- **Measurement-first debugging.** End-to-end voice latency decomposed on real devices (11.7s → 7.6s); a wrong suspicion (the STT stage) publicly retracted after measurement; TTS chunking identified as a 2.1× penalty and fixed with the trade-off cost recorded; ASR error baselined against the builder's own 20 hand-transcriptions (CER 28.2% / WER 59.8%), invalidating an earlier flattering number. **[FACT — repo-documented measurements]**
- **AI cost engineering.** Model-escalation ladders (cheap-first), local-catalog-before-API gating, batch/backoff embedding, real-usage token metering; one system's measured cost cut ~$4/day → ~$1.1/day. **[FACT — code + repo-documented measurements]**
- **Local AI under privacy constraints.** The builder's voice cloned entirely on his own GPU (OmniVoice zero-shot + Whisper large-v3), with biometric rules enforced *before* enabling direct-push: voice bytes never enter the repo; the phone path refuses to start without auth; "only my own voice is ever cloned." **[FACT — gitignore/commit ordering + auth code + policy in decisions log]**
- **Adversarial self-audit and correction.** A 19-area, 38-agent read-only audit of his own system produced 146 confirmed findings; 26 were fixed in test-green batches; an adversarial audit *of the fixes* found 4 real gaps, which were fixed; 120 findings deferred with written reasons. **[FACT — committed audit + fix reports, commits b8907dc→36eb96a, d0aef7b]**
- **Data governance.** Import runs preserved row-by-row with dispositions; cross-source dedup proven by 13,216 already-present hits on re-import; a live-proof document that includes its own three failed searches; image-rights refusals recorded by name. **[FACT — masterdatabase reports]**
- **Directing AI, not just using it.** 15+ documented cases where the builder caught the AI's errors — fabricated claims, overclaims, wrong architectural direction, stale docs — each with a root-cause confession recorded in the ledger; plus a founder-authored 326-line adversarial red-team report against an LLM whose structure became repo policy. **[FACT — audit-log entries; MAMA-OS reference doc]**
- **Verification-gated AI orchestration (2026-08-07).** The CI work that produced the machine-attested suites above was itself run under the builder's gates: plan shown first, writes only after approval, and the CI runtime version matched to the documented actual runtime at the builder's insistence; both pull requests were reviewed and merged by the builder. **[FACT — GitHub PR #112 / #82 records; gates visible in the PR bodies]**

## 4. Honest limits — stated plainly

- **No team history.** Structural, not chosen: there was no team to work with. Peer collaboration, receiving code review from humans, shared ownership — **[UNKNOWN]**. The closest existing analog — sustained review/gating of an AI collaborator across ~1,600 commits — is real but is an analog, not the thing itself. **[INFERENCE, labeled as such]**
- **Production-scale load has not yet been demonstrated.** Current deployment state: one real pharmacy in beta. **[FACT — deployment state; behavior under scale: UNKNOWN]**
- **Numbers outside the two CI'd repos are self-reported.** Test counts in other repos exist as files and documented runs but are not yet machine-attested. **[FACT — audit finding]**
- **Line-level authorship is not provable in either direction.** What is evidenced is system ownership: requirements, gates, verification, corrections. **[FACT — for the trail; INFERENCE — for skill attribution]**
- **Formal credentials, interview-condition fundamentals, English team-communication: [UNKNOWN].** Pre-June-2026 work exists by reference but is not verifiable (one referenced predecessor repo is empty). **[FACT — that it is unverifiable]**

## 5. Evidence-supported role fit (assessment, not aspiration)

The body of evidence maps most directly onto **applied-AI product engineering, forward-deployed/solutions engineering, voice-AI product work, and founding-/solo-engineer roles**; it does **not** currently support research-scientist or large-scale-infrastructure claims. **[INFERENCE — from the totality above, stated with the same restraint as the underlying audit]**

## 6. How to verify this document

1. Request the **full forensic audit report** (21 sections; every claim carries repo/path/SHA/date).
2. Request **read access** to any private repository named here — the ledgers and tests are in-tree.
3. Inspect the **public repositories** directly (visibility re-verified 2026-08-07): `DSE-AI-TRADER`, `cholo-jai`, `krishna-kanta`, `avijit-vaiya-portfolio`, `pharmacyos-website`.
4. Ask for the **GitHub Actions run links** for the two machine-attested suites (run IDs above).

*Published 2026-08-07 (v2 content, approved by the builder) · changes from v1: five corrections requested by the builder (section rename; mobile-operation claim re-tagged BUILDER-STATED; collaboration line softened to PR-record-backed facts; scale limit re-worded neutrally; public-repo visibility re-verified; "Verification-gated collaboration" renamed to "Verification-gated AI orchestration" at the builder's request). Nothing in this document was created after, or for, the evaluation it describes — except this document itself.*
