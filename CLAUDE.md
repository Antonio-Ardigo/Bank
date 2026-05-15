# CLAUDE.md — Authoring Guide for the Conventional Time Deposit Banking Manual

This file is the **builder's guide** for any Claude Code session that opens this repository. It is **not** the manual itself. The manual lives at `manual/MANUAL.md`.

If you are about to write, extend, review, or release any part of the manual, read this file first.

---

## 1. Project context

This repository holds the **Conventional Time Deposit Banking Manual** — a ~40-page, 10-chapter, 50-SOP operations manual for a commercial bank's conventional, interest-bearing time deposit product line.

- **Audience for the manual:** Branch Officers, Checkers, Branch Managers, Operations Controllers, Treasury Operations, Compliance and Financial Crime Officers, Finance and Reconciliation Accountants, Internal Audit, and external auditors under engagement.
- **Voice of the manual:** the formal, measured voice of a senior bank manager addressing peer professionals.
- **Success looks like:** a manual that an Internal Audit team or external auditor could pick up cold and rely on to test operating effectiveness.

## 2. Scope — in / out

**In scope (write about these):** conventional, interest-bearing time deposits — Certificates of Deposit (CDs), Term Deposits (TDs), Fixed Deposits (FDs) — across retail, private banking, SME, corporate, and institutional segments, in domestic and foreign currency.

**Out of scope (never write about these in the manual):**
- Islamic / Shariah-compliant deposit structures (Mudarabah, Wakalah, Qard, profit-sharing investment accounts)
- Structured deposits with embedded derivatives; market-linked deposits
- Demand deposits, savings deposits, notice deposits
- Insurance-wrapped savings; money-market funds
- Binding legal advice or specific named regulators / tax rates / insurance scheme limits treated as universal

## 3. Repository layout

```
/
├── CLAUDE.md            # This file — authoring guide for Claude Code
├── README.md            # (Optional) user-facing repo orientation
├── manual/
│   └── MANUAL.md        # CANONICAL manual — the single deliverable artifact
└── scripts/             # (Optional) acceptance-check scripts
```

**Current state:** the manual is maintained as a single file `manual/MANUAL.md`. Future sessions may, with PGC sign-off, split the manual into per-chapter sources under `manual/chapters/` and per-appendix sources under `manual/appendices/`, with `manual/MANUAL.md` becoming the assembled artifact. If you do this, **do not change SOP numbering or chapter taxonomy** in the process.

## 4. Chapter taxonomy (frozen)

The manual has exactly **10 chapters**. Titles and order are frozen; do not add, remove, or reorder chapters without a major version bump.

| Ch. | Title | One-line purpose |
|---|---|---|
| 1 | Foundations, Governance & Product Framework | Scope, 3LoD, PGC, roles, document control |
| 2 | Product Design, Pricing & Disclosure | Catalogue, ALCO rate setting, KFS, fees |
| 3 | Customer Onboarding, KYC & AML | CDD/EDD, screening, FATCA/CRS, red flags |
| 4 | Account Opening, Funding & Certificate Issuance | Mandate, funding channels, value-dating, maker-checker |
| 5 | Interest Accrual, Capitalisation & Day-Count Conventions | Day-count, simple/compound, accrual engine, WHT, GL postings |
| 6 | Rollover, Renewal & Mid-Term Events | Standing instructions, grace period, top-up/partial, pre-maturity advice |
| 7 | Early Withdrawal, Break Costs & Maturity Redemption | Break-cost formulae, hardship, payout, estate, lost certificate |
| 8 | Dormancy, Unclaimed Balances & Escheatment | Dormancy clock, tracing, statutory transfer, reactivation |
| 9 | Accounting, Reconciliation, Regulatory & Tax Reporting | CoA, subledger-to-GL, Basel/LCR, deposit insurance SCV, tax |
| 10 | Controls, Audit, Fraud, Complaints & Business Continuity | Control inventory, SoD, fraud typologies, IA cycle, complaints, BCP |

## 5. SOP numbering scheme (frozen — exactly 50 SOPs)

SOP numbers are **immutable**. Once an SOP is published it is never renumbered. A withdrawn SOP is marked `[Withdrawn]` in place. New SOPs append within the originating chapter's reserved range; if the range is full, raise a PGC amendment.

| Chapter | SOP range | Count |
|---|---|---|
| 1 | SOP-001 – SOP-004 | 4 |
| 2 | SOP-005 – SOP-009 | 5 |
| 3 | SOP-010 – SOP-017 | 8 |
| 4 | SOP-018 – SOP-023 | 6 |
| 5 | SOP-024 – SOP-029 | 6 |
| 6 | SOP-030 – SOP-033 | 4 |
| 7 | SOP-034 – SOP-039 | 6 |
| 8 | SOP-040 – SOP-043 | 4 |
| 9 | SOP-044 – SOP-048 | 5 |
| 10 | SOP-049 – SOP-050 | 2 |
| **Total** | | **50** |

## 6. Voice & style guide

Write in the formal, third-person institutional voice of a senior bank manager.

- **Subjects:** "the Bank", "the Officer", "the Branch", "the Operations Controller". Never "I", "we", "our", "us", "you" (except imperative inside SOP procedures, e.g., "the Officer shall...").
- **Normative force:**
  - **shall** — mandatory; departure is a control breach.
  - **should** — recommended; departure requires reasoned documentation.
  - **may** — permitted discretion within stated limits.
- **Vocabulary:** British/international banking English. Use *tenor* (not "term length"), *principal* (not "balance"), *accrual* (not "buildup"), *maturity proceeds*, *break cost*, *rollover instruction*, *dormant account*, *cheque*, *centre*, *subledger*.
- **Currency:** ISO 4217 with two decimals — `USD 10,000.00`, `EUR 1,500.00`. Never bare `$`, `£`, `€`.
- **Dates:** ISO 8601 — `YYYY-MM-DD`. Never `DD/MM/YYYY` or `MM/DD/YYYY`.
- **Rates:** per annum, two decimals — `4.25% p.a.`. Distinguish nominal from effective where compounding applies.
- **Numerals:** for control thresholds and timelines, give the word followed by the figure — "fourteen (14) days", "ninety (90) calendar days".
- **Tone:** measured, precise, risk-aware. Never marketing, never colloquial, no contractions ("don't", "can't"), no exclamation marks, no emojis.

## 7. The fixed SOP template

Every SOP **shall** contain, in order, exactly these eight fields, each on its own bolded line. No field may be omitted; where a field genuinely does not apply, write "Not applicable" with a one-line reason.

```
**SOP-### — Title in Title Case**
- **Purpose:** One sentence stating what the SOP exists to achieve.
- **Trigger:** The event that initiates the procedure.
- **Roles:** Maker — <role>; Checker — <role>; Approver — <role and threshold, if any>.
- **Inputs:** Documents, data, and prior approvals required.
- **Procedure:**
  1. First step.
  2. Second step.
  3. ...
- **Controls:** The specific control(s) embedded in this procedure. [Control Point]
- **Evidence:** The records to be retained. [Audit Evidence]
- **Reference:** Other SOPs, chapter sections, policies, regulations.
```

The Procedure field is a numbered list. The other seven fields are single-paragraph or short-list. Do not invent additional fields.

## 8. Standard call-outs

Use the following call-out tags, rendered in **bold square brackets**, at the end of the sentence they qualify. Do not invent new tags.

| Tag | When to use |
|---|---|
| `**[Jurisdiction-Dependent]**` | Any value, threshold, timeline, or rule set by local law, regulator, tax authority, insurance scheme, or accounting standard. **Every occurrence must also appear as a row in the Jurisdictional Parameters Workbook (Appendix C).** |
| `**[Audit Evidence]**` | Records the Bank must retain for external/internal audit examination. Tag the named artefact (form, log, ticket, minute). |
| `**[Red Flag]**` | A fraud, AML, or conduct indicator. Describe the indicator, not the response (the response lives in the Procedure). |
| `**[Control Point]**` | A control to be tested under the RCSA programme. One control per tag; control must be testable and observable. |

## 9. Formulas, day-count examples, and journal entries

**Formulas.** Short inline forms in backticks: `I = P × r × (t / B)`. Multi-line derivations in fenced code blocks. Every worked example carries an explicit *Assumptions* line stating principal, rate, tenor, day-count, currency, and value date.

**Day-count conventions.** When introducing or applying a convention, name it explicitly: `30/360`, `ACT/360`, `ACT/365 Fixed`, `ACT/ACT`. Show the same worked example across conventions when comparing.

**Journal entries.** Always rendered as fixed-width fenced code blocks in the canonical Dr / Cr / Amount / Narrative layout, with illustrative GL codes (real codes are configured in the Bank's Chart of Accounts):

```
Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
   Cr  1110-CASA-CUST                         USD 100,000.00
Narrative: Funding of TD #TD-2026-000123, 12M, 4.25% p.a.
```

## 10. Cross-referencing

Refer to other parts of the manual by **stable identifier**, never by page number:

- SOPs: `SOP-027`
- Chapter sections: `Ch. 6 sec. 6.3`
- Appendices: `Appendix C, row C-014`

Every cross-reference must resolve by grep. If you cite `SOP-027`, that SOP header must exist somewhere in the manual.

## 11. Jurisdictional values — the placeholders workbook pattern

The manual is jurisdiction-neutral. Local Compliance and Legal populate values for their territory.

- In chapter prose, write the rule **abstractly** and tag it `**[Jurisdiction-Dependent]**`. Do **not** embed the local number, rate, or statute name.
- Add a corresponding row in the **Jurisdictional Parameters Workbook** (Appendix C of `manual/MANUAL.md`) in the same change, with columns: *Ref · Item · Source · Value (to be populated)*.
- Every chapter ends with this exact closing line:

  > *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

## 12. Word-budget and pagination (~40 pages, ~500 words per page rendered)

| Chapter | Target words | Tolerance |
|---|---|---|
| Front matter (foreword, ToC, how-to-read) | 600 | ±20% |
| Ch. 1 | 1,600 | ±15% |
| Ch. 2 | 1,800 | ±15% |
| Ch. 3 | 2,400 | ±15% |
| Ch. 4 | 1,800 | ±15% |
| Ch. 5 | 2,000 | ±15% |
| Ch. 6 | 1,600 | ±15% |
| Ch. 7 | 2,000 | ±15% |
| Ch. 8 | 1,400 | ±15% |
| Ch. 9 | 2,400 | ±15% |
| Ch. 10 | 2,000 | ±15% |
| Appendices A–F | not counted toward the 40-page body | — |

Over-budget chapters must be **trimmed**, not allowed to bleed into other chapters.

## 13. Adding new content without breaking the manual

- **New SOP:** must fit within the originating chapter's reserved SOP range (§5). If the range is full, raise a PGC amendment — either replace a withdrawn SOP or expand the range. Never re-use a number; never renumber existing SOPs.
- **New chapter:** requires PGC approval and a major version bump. Chapter taxonomy is otherwise frozen.
- **New appendix:** append with the next available letter (G, H, …). Existing letter assignments are immutable.
- **New term:** define on first use; add a row to Appendix A (Glossary) in the same change.
- **New acronym:** expand on first use; add to Appendix B in the same change.

## 14. Review, approval, and version control

- Every change cites the Product Programme Document (PPD) reference touched and the Product Governance Committee (PGC) minute number authorising the change.
- Every released version is stamped in Appendix F (Document Control & Version History) with: version, effective date, summary of change, approver, supersession note.
- Versioning:
  - `1.0.1` — editorial fixes, no normative change
  - `1.1` — clause amendments
  - `2.0` — taxonomy changes (chapter or appendix structure)

## 15. What the manual must NEVER contain

- Islamic / Shariah structures or terminology (Mudarabah, Wakalah, Qard, riba, halal, profit-sharing investment accounts)
- Binding legal advice (e.g., "you must under section X of [Act]")
- Specific named regulators, central banks, deposit insurance schemes, tax rates, or statutory limits treated as universal
- Marketing language ("best rates", "competitive", "exclusive", "market-leading")
- First-person voice ("I", "we", "our team")
- Contractions ("don't", "can't"), exclamation marks, emojis
- Platform-specific screenshots or vendor names treated as the standard
- Customer-identifying data or internal pricing taken from production systems

## 16. Example block — copy this shape exactly

> **SOP-027 — Back-Value Adjustment and Interest Recomputation**
> - **Purpose:** Correct dated errors discovered after the event without distorting the audit trail.
> - **Trigger:** Error in tenor, rate, day-count, or principal identified after accrual has commenced.
> - **Roles:** Maker — Branch Officer or Operations Officer; Checker — Operations Controller; Approver — Head of Finance Operations.
> - **Inputs:** Root-cause analysis; corrected accrual computation; customer-impact statement.
> - **Procedure:**
>   1. The originator submits the back-value request with supporting evidence.
>   2. Operations recomputes the accrual from the original value date to the date of correction.
>   3. Reversal and re-booking entries are posted with the back-value flag; the customer is informed where their net position changes.
>   4. The case is logged in the operational incident register.
> - **Controls:** Threshold-based escalation to the Operating Risk Committee; quarterly trend review. **[Control Point]**
> - **Evidence:** Adjustment request; GL entries; customer notification. **[Audit Evidence]**
> - **Reference:** Ch. 5 sec. 5.7; Appendix D — Sample Journal Entries; Operational Incident Policy.

Canonical journal-entry block:

```
Dr  2215-TD-INT-PAYABLE                 USD     50.00
   Cr  8110-INT-EXP-TD                          USD     50.00
Narrative: Back-value reversal of over-accrual on TD #TD-2026-000123
```

Inline call-out usage:

> The Bank shall transfer unclaimed balances to the designated public fund upon expiry of the statutory dormancy window. **[Jurisdiction-Dependent]** The transfer file shall be retained for the period prescribed by the relevant authority. **[Audit Evidence]** A reconciliation between the dormancy register and the transferred file is performed by an officer independent of dormancy operations. **[Control Point]** A customer claim arriving after transfer shall be treated as a potential impersonation indicator until identity is re-verified. **[Red Flag]**

## 17. Pre-write checks (run before drafting)

1. Identify the target chapter and confirm its reserved SOP range has capacity (§5).
2. Read the surrounding sections of `manual/MANUAL.md` to inherit voice, vocabulary, and abbreviation choices.
3. Locate cross-references that may need updating; plan the same-PR changes (glossary, acronyms, Appendix C, Appendix E).
4. Confirm the change has — or will have — a PPD reference and PGC minute number.

## 18. Post-write self-check (run before declaring a change complete)

Automated greps:

```bash
# 1. Exactly 50 SOPs
grep -hoE '^\*\*SOP-[0-9]{3}' manual/MANUAL.md | sort -u | wc -l   # → 50

# 2. SOPs are contiguous SOP-001..SOP-050
grep -hoE 'SOP-[0-9]{3}' manual/MANUAL.md | sort -u | head; \
grep -hoE 'SOP-[0-9]{3}' manual/MANUAL.md | sort -u | tail        # → first 001, last 050

# 3. Every chapter ends with the jurisdictional reminder line
grep -c 'Local Compliance and Legal shall confirm all jurisdictional parameters' manual/MANUAL.md   # → 10

# 4. No prohibited Islamic-banking terminology
grep -riE '\b(mudarabah|wakalah|qard|shariah|halal|riba)\b' manual/   # → empty

# 5. No emojis
grep -P '[\x{1F300}-\x{1FAFF}\x{2600}-\x{27BF}]' manual/   # → empty

# 6. No marketing language
grep -riE '\b(best rates?|exclusive|competitive|market-leading|unbeatable)\b' manual/   # → empty

# 7. No bare currency symbols
grep -nE '[$£€]' manual/MANUAL.md   # → empty

# 8. No non-ISO date formats
grep -nE '\b[0-9]{2}/[0-9]{2}/[0-9]{4}\b' manual/MANUAL.md   # → empty
```

Manual reviewer checks:

- Every SOP block has all eight required fields (Purpose, Trigger, Roles, Inputs, Procedure, Controls, Evidence, Reference).
- Every `**[Jurisdiction-Dependent]**` occurrence has a corresponding row in Appendix C.
- Every newly introduced term is in Appendix A; every newly introduced acronym is in Appendix B.
- Appendix E (SOP Index) lists exactly 50 rows.
- Appendix F (Document Control) carries a row for the version being released.
- Chapter word counts are within ±15% of the §12 targets.
- All cross-references (`SOP-NNN`, `Ch. N sec. N.N`, `Appendix X, row Y`) resolve.

## 19. DO / DON'T cheat sheet

**DO**
- Write in third-person, formal, bank-manager voice.
- Use *shall / should / may* deliberately.
- Use ISO 4217 (`USD 10,000.00`) and ISO 8601 (`YYYY-MM-DD`).
- Keep every SOP to the 8-field template.
- Tag jurisdictional items `**[Jurisdiction-Dependent]**` and add the Appendix C row in the same change.
- Cross-reference by `SOP-NNN`, `Ch. N sec. N.N`, or `Appendix X, row Y`.
- Trim to the word budget.

**DON'T**
- Use first-person voice ("I", "we", "our").
- Reference Islamic / Shariah structures.
- Give binding legal advice or quote specific regulators / tax rates / insurance limits as universal.
- Use marketing language.
- Use emojis, exclamation marks, or contractions.
- Renumber existing SOPs.
- Embed jurisdictional values inline in chapter prose.
- Cross-reference by page number.
