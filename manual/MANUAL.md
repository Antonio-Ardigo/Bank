# Conventional Time Deposit Banking Manual

**Document title:** Conventional Time Deposit Banking Manual
**Document owner:** Head of Retail & Wholesale Liabilities
**Approved by:** Asset & Liability Committee (ALCO) and the Product Governance Committee
**Classification:** Internal — Restricted to authorised staff and external auditors under engagement
**Version:** 1.0
**Effective date:** Upon issuance under the seal of the Board Secretariat
**Review cycle:** Annual, or upon material change in product, regulation, or core banking platform

---

## Foreword by the Bank Manager

The acceptance of a time deposit is the most ordinary, and the most consequential, transaction the Bank performs. Ordinary, because thousands of such deposits are booked across our branches every day. Consequential, because every certificate issued is, in substance, the Bank's solemn promise to repay a sum of money, with interest, on a date certain. Behind that single promise stand the Bank's liquidity, its reputation, its regulatory standing, and the trust of the depositor.

This manual codifies how the Bank originates, services, accounts for, and ultimately discharges that promise across the full lifecycle of a conventional, interest-bearing time deposit. It is written for the Officer at the counter, the Checker at the back office, the Branch Manager who authorises the exception, the Treasury dealer who funds the book, the Accountant who reconciles the ledger, the Compliance Officer who clears the screening hit, and the Auditor who, in due course, will examine the evidence we leave behind.

Read it. Apply it. When in doubt, escalate. The Bank's good name rests upon the diligence with which these pages are observed.

— *The Bank Manager*

---

## Table of Contents

1. **Chapter 1 — Foundations, Governance & Product Framework**
2. **Chapter 2 — Product Design, Pricing & Disclosure**
3. **Chapter 3 — Customer Onboarding, KYC & AML**
4. **Chapter 4 — Account Opening, Funding & Certificate Issuance**
5. **Chapter 5 — Interest Accrual, Capitalisation & Day-Count Conventions**
6. **Chapter 6 — Rollover, Renewal & Mid-Term Events**
7. **Chapter 7 — Early Withdrawal, Break Costs & Maturity Redemption**
8. **Chapter 8 — Dormancy, Unclaimed Balances & Escheatment**
9. **Chapter 9 — Accounting, Reconciliation, Regulatory & Tax Reporting**
10. **Chapter 10 — Controls, Audit, Fraud, Complaints & Business Continuity**

**Appendices**
- A. Glossary
- B. Acronym List
- C. Jurisdictional Parameters Workbook
- D. Sample Journal Entries — Consolidated
- E. SOP Index (1–50)
- F. Document Control & Version History

---

## How to Read This Manual

- **"Shall"** denotes a mandatory act. Departure constitutes a control breach and shall be logged as an incident.
- **"Should"** denotes recommended practice. Departure shall be reasoned and documented.
- **"May"** denotes permitted discretion within stated limits.
- **SOPs** are presented in a fixed structure: *Purpose · Trigger · Roles (Maker / Checker / Approver) · Inputs · Procedure · Controls · Evidence · Reference.*
- Currency amounts are expressed in ISO 4217 (e.g., USD 10,000.00). Dates are expressed in ISO 8601 (YYYY-MM-DD). Rates are expressed per annum to two decimal places (e.g., 4.25% p.a.).
- The following call-outs appear throughout:
  - **[Jurisdiction-Dependent]** — item depends on local law, regulator, deposit insurance scheme, tax authority, or accounting standard.
  - **[Audit Evidence]** — record to be retained for examination.
  - **[Red Flag]** — fraud or AML indicator.
  - **[Control Point]** — control to be tested under the RCSA programme.

---

# Chapter 1 — Foundations, Governance & Product Framework

## 1.1 Scope, Audience, and How to Use This Manual

This manual governs the conventional, interest-bearing time deposit product line of the Bank, comprising certificates of deposit (CDs), term deposits (TDs), and fixed deposits (FDs), in domestic and foreign currency, offered to retail, private banking, small business, corporate, and institutional clients of the Bank. It is the single operational reference for the origination, servicing, accounting, regulatory reporting, and closure of these instruments.

This manual does not govern Islamic or profit-sharing deposit structures (Mudarabah, Wakalah, Qard-based products), which are addressed in a separate Shariah Banking Manual. It does not govern structured deposits with embedded derivatives, market-linked deposits, money-market mutual funds, or insurance-wrapped savings products, all of which fall under distinct product programmes. Demand deposits, savings deposits, and notice deposits are likewise out of scope.

The audience comprises front-office Officers and Branch Managers, back-office Operations and Treasury Operations staff, Compliance and Anti-Financial-Crime Officers, Finance and Reconciliation Accountants, Internal Audit, and the external auditors of the Bank under engagement. New joiners shall complete the induction module on this manual within thirty (30) days of assuming duties.

## 1.2 Definition of Conventional Time Deposits

A conventional time deposit is a contract under which the depositor places a stated principal sum with the Bank for a stated tenor at a stated interest rate, with the Bank's promise to repay the principal together with accrued interest at maturity. The defining features are: (a) a fixed principal, (b) a fixed tenor, (c) a contractual interest rate determined at inception, (d) limited or no liquidity prior to maturity, and (e) the Bank's unconditional obligation to repay irrespective of the use to which the funds are put.

The product line is broken into three reporting families: short-dated TDs (tenor up to and including 92 days), medium-dated TDs (tenor 93 days up to and including 366 days), and long-dated TDs (tenor exceeding 366 days, capped at the maximum tenor approved in the Product Programme Document). Foreign currency TDs are tracked in a separate reporting dimension.

## 1.3 Three Lines of Defence Model

The Bank operates a three-lines-of-defence model in respect of the time deposit book. The **First Line (1LoD)** comprises the Branch and Operations staff who own and execute the daily control activities embedded in the procedures of this manual. The **Second Line (2LoD)** comprises Risk Management, Compliance, and Financial Crime, which set policy, set risk appetite, independently monitor first-line execution, and perform thematic testing. The **Third Line (3LoD)** is Internal Audit, which provides independent assurance to the Board Audit Committee on the design and operating effectiveness of the control environment.

No control may be owned and tested by the same line. Where the Operations function reconciles a balance, the test of that reconciliation is performed by Risk or Internal Audit, never by Operations.

## 1.4 Product Governance Committee and Approval Authorities

The Product Governance Committee (PGC) is the standing forum that approves the introduction, material amendment, and decommissioning of any time deposit product. The PGC is chaired by the Head of Liabilities and is attended by representatives of Risk, Compliance, Finance, Legal, Operations, Technology, and Internal Audit (the latter in observer capacity). No conventional time deposit product, tenor, currency, or rate structure may be offered to customers without an approved Product Programme Document (PPD) bearing the PGC's seal and a fresh review not older than twelve (12) months.

Approval authorities for routine pricing actions are delegated to the ALCO under a separate Delegations of Authority schedule. Exceptional pricing (preferential rates) is governed by SOP-009.

**RACI — Product Governance**

| Lifecycle Stage | Product Mgr | ALCO | Risk | Compliance | Finance | Ops | Internal Audit |
|---|---|---|---|---|---|---|---|
| New product design | R | C | C | C | C | C | I |
| Product approval | A | A | C | C | C | C | I |
| Pricing (rate sheet) | R | A | C | I | I | I | I |
| Disclosure language | R | I | I | A | I | C | I |
| Operational readiness | R | I | C | C | C | A | I |
| Annual product review | A | C | C | C | C | C | I |
| Product decommissioning | A | C | C | C | C | C | I |

*R = Responsible, A = Accountable, C = Consulted, I = Informed.*

## 1.5 Roles, Titles, and Segregation of Duties (Overview)

The following titles are used throughout this manual and reflect functional, not necessarily hierarchical, roles:

- **Officer (Maker):** Front-line staff who initiate a transaction in the core banking system.
- **Checker:** Independent staff member at the same or higher grade who reviews the maker's entries before they take effect.
- **Approver:** Authorised signatory whose mandate is established under the Bank's Delegations of Authority and who releases the transaction.
- **Branch Manager:** Accountable for control execution within the branch.
- **Operations Controller:** Back-office head accountable for end-of-day processing of the TD book.
- **Treasury Operations:** Settles funding flows and books FX legs for foreign currency TDs.
- **Compliance Officer:** Reviews KYC, sanctions, and regulatory matters.
- **Reconciler:** Finance staff accountable for the daily TD subledger-to-GL reconciliation.

No single individual shall both initiate and authorise a customer-facing transaction in the time deposit book, save under the documented emergency-access procedures described in Chapter 10.

## 1.6 Document Control, Version History, and Waiver Process

This manual is the property of the Bank and is maintained under document control by the Manual Custodian (Operations Policy team). Only the version published on the official Bank intranet is authoritative. Printed copies are uncontrolled and may not be relied upon beyond the date printed on the footer.

Material changes shall be approved by the PGC and re-issued under a new version number. Minor editorial corrections may be released under a sub-version (e.g., 1.0.1) with a note in the change log. All staff acting in any of the roles named in section 1.5 shall acknowledge each new version within fourteen (14) days of release.

Where a business need arises that cannot be met within this manual, a written waiver shall be requested under SOP-003. Verbal waivers are not recognised by the Bank.

### Standard Operating Practices in this Chapter

---

**SOP-001 — New Product Approval and Product Programme Document Issuance**
- **Purpose:** Ensure no time deposit product is offered to customers without documented, multi-disciplinary approval and operational readiness.
- **Trigger:** Proposal to introduce a new tenor, currency, customer segment, channel, or rate structure.
- **Roles:** Maker — Product Manager; Checker — Risk Manager and Compliance Officer; Approver — Product Governance Committee.
- **Inputs:** Draft Product Programme Document (PPD); market study; risk assessment; legal opinion; operational readiness checklist; system change request.
- **Procedure:**
  1. The Product Manager drafts the PPD covering customer segment, eligibility, tenor, currency, rate methodology, fees, disclosures, accounting treatment, regulatory treatment, controls, and decommissioning plan.
  2. Second-line reviewers (Risk, Compliance, Legal, Finance) submit written sign-off or reasoned objection within ten (10) business days.
  3. Operations and Technology confirm system readiness, including GL mapping, accrual engine configuration, certificate template, and reconciliation feed.
  4. The PGC tables the PPD; the Chair records the decision and conditions, if any.
  5. The Manual Custodian updates the product catalogue and disclosure registry.
- **Controls:** No product code may be activated in the core banking system without an approved PPD reference on file. **[Control Point]**
- **Evidence:** Signed PPD, PGC minutes, system change ticket, disclosure registry entry. **[Audit Evidence]**
- **Reference:** Product Governance Charter; Delegations of Authority.

---

**SOP-002 — Annual Product Review and Product-Line Attestation**
- **Purpose:** Confirm that every live time deposit product remains fit for purpose, profitable, and compliant.
- **Trigger:** Annual product review cycle; ad hoc following material regulatory change.
- **Roles:** Maker — Product Manager; Checker — Finance and Risk; Approver — PGC.
- **Inputs:** Twelve-month performance MIS; complaint trends; conduct metrics; control breach log; competitor scan; regulatory horizon scan.
- **Procedure:**
  1. The Product Manager prepares the Annual Product Review pack per product.
  2. Finance attaches profitability and net interest margin (NIM) contribution.
  3. Risk and Compliance attach incidents, complaints, and regulatory observations.
  4. The PGC resolves to *retain, amend, restrict, or decommission* each product.
  5. The decision is reflected in the product catalogue and, where amendment is approved, triggers a refreshed PPD via SOP-001.
- **Controls:** Any product not reviewed within thirteen (13) months from the prior review shall be flagged red on the product catalogue and suspended to new business. **[Control Point]**
- **Evidence:** Annual Product Review pack; PGC minutes; updated catalogue. **[Audit Evidence]**
- **Reference:** Product Governance Charter section 4.

---

**SOP-003 — Policy Waiver Request, Approval, and Logging**
- **Purpose:** Permit time-limited departures from this manual where business need is demonstrated, without normalising non-compliance.
- **Trigger:** Officer or Branch Manager identifies a transaction that cannot proceed within the four corners of this manual.
- **Roles:** Maker — Officer/Branch Manager; Checker — Compliance Officer; Approver — Head of Liabilities (or higher, per matter).
- **Inputs:** Waiver request form stating clause to be waived, business justification, customer impact, risk mitigants, expiry date.
- **Procedure:**
  1. The requester completes the waiver form and routes it via the waiver registry.
  2. Compliance reviews for regulatory permissibility; Risk reviews for residual risk.
  3. Approver records decision (Granted / Granted with conditions / Refused) and expiry, which shall not exceed ninety (90) days.
  4. Waiver register is updated; expiring waivers are alerted to the original requester at T-7.
- **Controls:** Waivers granted under emergency authority shall be ratified within five (5) business days. Repeated waivers on the same clause shall trigger a manual amendment proposal. **[Control Point]**
- **Evidence:** Waiver register entry; approver email or signed form. **[Audit Evidence]**
- **Reference:** Operational Risk Framework section on policy exceptions.

---

**SOP-004 — Manual Maintenance, Versioning, and Staff Acknowledgement**
- **Purpose:** Ensure the manual remains current, that staff act upon the current version, and that acknowledgement is auditable.
- **Trigger:** Material amendment; annual review; regulatory change; PGC decision.
- **Roles:** Maker — Manual Custodian; Checker — Compliance; Approver — Head of Liabilities.
- **Inputs:** Change log; redline draft; impact assessment.
- **Procedure:**
  1. The Custodian maintains a change log indexed by clause.
  2. Each new version is published on the intranet under a unique version number.
  3. The training platform issues an acknowledgement task to all named role-holders.
  4. Non-acknowledgement after fourteen (14) days is escalated to the line manager and, after twenty-one (21) days, to Human Resources.
- **Controls:** Quarterly attestation report to the Operating Risk Committee. **[Control Point]**
- **Evidence:** Change log; acknowledgement audit trail. **[Audit Evidence]**
- **Reference:** Document Control Policy.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 2 — Product Design, Pricing & Disclosure

## 2.1 Product Catalogue: Tenors, Currencies, Minimums, and Tiers

The Bank's conventional time deposit catalogue defines the product matrix permitted to be sold. Every product code in the core banking system shall correspond to a row in this catalogue and to an active Product Programme Document. The illustrative structure of the catalogue is given below; specific values are set in the published catalogue and shall not be assumed from this manual.

**Illustrative Product Catalogue Structure**

| Field | Description | Example |
|---|---|---|
| Product code | Internal CBS identifier | TD-DOM-12M-RTL |
| Customer segment | Retail / Private / SME / Corporate / Institutional | Retail |
| Currency | ISO 4217 | USD |
| Minimum principal | Per tier | USD 1,000.00 |
| Maximum principal | Per tier (above which approval required) | USD 1,000,000.00 |
| Tenor | Calendar days, weeks, months, or years | 12 months |
| Rate basis | Fixed / Step-up / Promotional | Fixed |
| Interest payment | At maturity / Monthly / Quarterly / Capitalised | At maturity |
| Early withdrawal | Permitted Y/N; method | Y — interest forfeiture |
| Channel | Branch / Digital / Relationship Manager | Branch + Digital |

**[Jurisdiction-Dependent]** Foreign currency offerings require an FX permit; non-resident customer offerings require capital-account permissibility under local exchange control regulation.

## 2.2 Interest Rate Setting: ALCO Mandate and Rate Sheet Cycle

Interest rates on conventional time deposits are set by the Treasury function under an ALCO-approved methodology. The methodology shall reflect, at minimum: (a) the Bank's funding need across tenors, as projected in the funding plan; (b) prevailing wholesale market rates for the corresponding tenor; (c) competitive positioning within the market; (d) regulatory floors and ceilings, where applicable; (e) net interest margin targets; and (f) liquidity coverage and funding stability considerations under Basel standards.

Rates are published in a rate sheet on a weekly cadence, or more frequently in response to market events, and are effective at the start of the next business day. The historical rate sheet archive shall be retained for a period not less than seven (7) years.

## 2.3 Promotional Rates, Bonus Rates, and Step-Up Products

Promotional and bonus rate offers are governed by a separate campaign approval that supplements the underlying PPD. Each campaign shall have a defined start date, end date, target segment, and total funding cap. Campaign rates shall not be evergreen; an undated campaign shall not be approved.

Step-up products, in which the contractual rate rises at pre-defined intervals within the tenor, shall display the schedule of step-up dates and rates on the Key Facts Statement, the customer advice, and the certificate. The accrual engine shall be configured to apply the schedule automatically.

## 2.4 Customer Disclosure: Key Facts Statement (KFS) and Terms & Conditions

A Key Facts Statement shall be presented to every customer prior to the conclusion of a time deposit contract. The KFS shall be a stand-alone document, not embedded within marketing material, and shall set out, at minimum: the product name, the contractual interest rate (nominal and effective), the day-count convention, the tenor and maturity date, the maturity instruction at booking, the consequences of early withdrawal including the break-cost methodology, the applicability of withholding tax, the protection (if any) afforded by the deposit insurance scheme, the Bank's complaint channels, and the customer's right to cancel within any cooling-off period.

> **Sample Disclosure Language — Opening of the KFS**
>
> *"This Key Facts Statement summarises the principal features of the time deposit product you are about to open with the Bank. It is provided in addition to, and does not replace, the full Terms and Conditions, a copy of which has been furnished to you. You are invited to read this statement carefully before signing the deposit application."*

> **Sample Disclosure Language — Break-Cost Clause**
>
> *"You may request early termination of this deposit before its maturity date. If the Bank in its discretion accepts your request, the proceeds payable to you will be reduced by a break cost calculated in accordance with the methodology disclosed in this statement, and the interest you ultimately receive may be materially less than, or zero, compared with the contractual rate."*

> **Sample Disclosure Language — Auto-Rollover Consent**
>
> *"Unless you instruct the Bank otherwise in writing not later than the maturity date, this deposit will, at maturity, be automatically renewed for an equal tenor at the prevailing rate then offered by the Bank for that tenor."*

## 2.5 Fee Schedule and Break-Cost Disclosure

The fee schedule applicable to the time deposit book shall be published alongside the rate sheet. Permissible charges shall be limited to those approved in the PPD and shall include, where applicable, certificate replacement fees, early withdrawal handling fees (distinct from the financial break cost), and statement reproduction fees. Fees not in the published schedule shall not be levied.

The break-cost methodology shall be disclosed in the KFS in plain language, supplemented by a worked example. The Bank applies, by default, an interest-forfeiture methodology calibrated to elapsed tenor; reinvestment-loss methodology is reserved for wholesale and institutional segments where contractually agreed.

## 2.6 Cross-Border and Foreign Currency TD Considerations

Foreign currency time deposits are subject to additional considerations: customer eligibility under exchange control regulations, FX confirmation for the principal leg, FX risk acknowledgement by the customer, the absence (in many jurisdictions) of deposit insurance protection on foreign currency balances, and currency-specific accrual conventions. Cross-border deposits placed by non-resident customers raise additional KYC, tax, and reporting considerations addressed in Chapters 3 and 9.

### Standard Operating Practices in this Chapter

---

**SOP-005 — Daily/Weekly Rate Sheet Preparation, ALCO Sign-Off, and Branch Distribution**
- **Purpose:** Ensure rates offered to customers are current, approved, and consistent across channels.
- **Trigger:** End-of-day on rate-setting day; ad hoc market event.
- **Roles:** Maker — Treasury Pricing Analyst; Checker — Head of Treasury; Approver — ALCO Chair or delegated rate-setting authority.
- **Inputs:** Wholesale market rate inputs; funding plan; competitor scan; regulatory rate constraints, if any.
- **Procedure:**
  1. Pricing Analyst computes the proposed rate grid for all live products.
  2. Head of Treasury reviews against funding need and NIM.
  3. ALCO Chair or delegate signs off the published rate sheet; the sign-off is recorded.
  4. The signed rate sheet is uploaded to the core banking pricing module and is broadcast to branches with a confirmation-of-receipt task.
  5. The previous rate sheet is archived in the rate registry.
- **Controls:** A reconciliation between the rate sheet PDF, the CBS pricing table, and the digital banking display is run end-of-day to detect drift. **[Control Point]**
- **Evidence:** Signed rate sheet; CBS configuration log; branch acknowledgements. **[Audit Evidence]**
- **Reference:** ALCO Charter; Pricing Policy.

---

**SOP-006 — Promotional/Campaign Rate Approval and Expiry Control**
- **Purpose:** Govern bonus and promotional rates as time-bound, capped offerings.
- **Trigger:** Marketing proposal for a campaign.
- **Roles:** Maker — Product Manager; Checker — Compliance, Finance; Approver — PGC delegate.
- **Inputs:** Campaign brief specifying segment, tenor, rate, cap, start/end dates, disclosure copy.
- **Procedure:**
  1. The campaign brief is submitted with a draft of all customer-facing material.
  2. Compliance confirms the disclosure language; Finance confirms the funding cap.
  3. The approved campaign is uploaded as a time-limited product code or rate override in the CBS.
  4. The CBS automatically blocks bookings against the campaign rate after the end date.
  5. A post-campaign report is tabled at the next PGC.
- **Controls:** Funded volume against the cap is monitored daily; bookings beyond ninety (90) percent of cap trigger Treasury notification. **[Control Point]**
- **Evidence:** Campaign brief; PGC approval; daily volume report; post-campaign review. **[Audit Evidence]**
- **Reference:** Pricing Policy.

---

**SOP-007 — Key Facts Statement Issuance and Customer Acknowledgement**
- **Purpose:** Ensure every depositor receives, and acknowledges, the KFS before the deposit is booked.
- **Trigger:** Customer applies for a new time deposit.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — implicit upon customer signature.
- **Inputs:** Approved KFS template; product code; customer particulars.
- **Procedure:**
  1. Officer prints or displays the KFS populated for the specific transaction (principal, rate, tenor, maturity date, fees).
  2. Officer walks the customer through each section.
  3. Customer signs (wet or digital) acknowledging receipt and understanding.
  4. The signed KFS is uploaded into the customer's digital file and the reference is captured against the deposit account.
- **Controls:** No deposit may be activated in the CBS without a KFS reference on file. **[Control Point]**
- **Evidence:** Signed KFS in the document management system. **[Audit Evidence]**
- **Reference:** Consumer Disclosure Policy.

---

**SOP-008 — Foreign Currency TD Eligibility Check and FX Confirmation**
- **Purpose:** Validate customer eligibility for foreign-currency deposits and confirm the FX leg.
- **Trigger:** Customer requests an FCY time deposit.
- **Roles:** Maker — Branch Officer; Checker — Branch FX Authoriser; Approver — Operations Controller for amounts above the branch threshold.
- **Inputs:** Customer KYC; residency status; FCY funding source; FX rate quote.
- **Procedure:**
  1. Officer confirms residency / non-residency and eligibility under prevailing exchange control rules.
  2. If FX conversion is required, Treasury Operations confirms the dealing rate within the dealing-rate band.
  3. Customer signs the FX confirmation and an acknowledgement of FCY risk.
  4. The deposit is booked using the FCY product code; the conversion leg is booked separately.
- **Controls:** End-of-day FCY position is reconciled to the dealing system. **[Control Point]**
- **Evidence:** FX confirmation; customer acknowledgement; dealing slip. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Exchange Control regulation; FX Dealing Policy.

---

**SOP-009 — Rate-Exception (Preferential Pricing) Approval and Logging**
- **Purpose:** Govern departures from the published rate sheet for individual depositors.
- **Trigger:** Relationship Manager requests a rate exception above the standard grid.
- **Roles:** Maker — Relationship Manager; Checker — Branch Manager; Approver — Treasury for limits up to a threshold, Head of Liabilities above.
- **Inputs:** Exception request stating customer, principal, tenor, requested rate, justification, expected total relationship value.
- **Procedure:**
  1. RM submits the exception request specifying the spread over the published rate.
  2. Treasury confirms whether the exception falls within the daily exception budget.
  3. The Approver records approval (or refusal) with conditions.
  4. The exception is logged in the exception registry; the booking uses the approved override rate in the CBS, which is flagged in MIS.
- **Controls:** Aggregate exception volume is reported daily to ALCO; chronic exception users are subject to relationship review. **[Control Point]**
- **Evidence:** Exception request; approver record; CBS override flag. **[Audit Evidence]**
- **Reference:** Delegations of Authority; Pricing Policy.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 3 — Customer Onboarding, KYC & AML

## 3.1 Customer Categories and Eligibility

The Bank accepts time deposits from the following customer categories: natural persons (resident individuals, non-resident individuals, minors through guardians, joint holders, persons acting under power of attorney), legal persons (corporations, partnerships, limited liability companies, sole proprietorships), trusts and foundations, unincorporated associations and clubs, financial institutions, and government and public-sector entities. Each category has its own onboarding pack, signatory mandate template, and beneficial-ownership disclosure requirement.

Eligibility is determined by reference to the Bank's risk appetite statement, customer acceptance policy, and prevailing financial-crime sanctions and embargoes. No customer who is the subject of a sanction administered in a jurisdiction in which the Bank operates may be onboarded.

## 3.2 CDD, EDD, and Simplified DD Triggers

The Bank applies a risk-based approach to customer due diligence. Standard Customer Due Diligence (CDD) applies to the great majority of customer relationships and requires the verification of identity and address using independent and reliable source documents.

Enhanced Due Diligence (EDD) is mandated where the customer or transaction presents elevated risk, including but not limited to: politically exposed persons (PEPs) and their close associates, customers from or with significant activity in high-risk jurisdictions, complex ownership structures, cash-intensive businesses, non-resident customers without a clear nexus to the Bank's market, and any case where customary CDD has produced an unsatisfactory result.

Simplified Due Diligence (SDD) is permitted only where expressly authorised by Compliance and only for product-customer combinations of demonstrably low risk; it shall not apply to deposits sourced from cash above the cash transaction reporting threshold.

## 3.3 Beneficial Ownership and Source-of-Funds / Source-of-Wealth

For all legal persons and arrangements, the ultimate beneficial owner (UBO) shall be identified to the natural-person level; ownership thresholds shall not exceed the lower of the local statutory threshold or twenty-five percent (25%), but the Bank reserves the right to apply a lower threshold where opacity warrants.

For deposits of significant size, irrespective of customer type, the Bank shall obtain evidence of source of funds (the immediate origin of the money being deposited) and, in EDD cases, source of wealth (the broader economic basis for the customer's accumulated assets). Self-declaration alone is insufficient; corroborating evidence (payslips, sale-of-asset documents, inheritance papers, audited financials) shall be reviewed and retained.

## 3.4 PEP, Sanctions, and Adverse Media Screening

Every prospective customer, every UBO, every authorised signatory, and every counterparty in a deposit-related transaction shall be screened against (a) sanctions and watch lists relevant to the jurisdictions in which the Bank operates, (b) PEP lists, and (c) adverse media at a level calibrated to risk. Hits shall be cleared by the second-line Financial Crime team; cleared hits and their reasoning shall be retained. Unresolved hits prohibit onboarding.

## 3.5 KYC Risk Rating Matrix and Periodic Refresh

Each customer is assigned a KYC risk rating at onboarding and reassessed periodically. The risk rating is the function of customer-type risk, geographic risk, product/channel risk, and behavioural risk.

**KYC Risk Matrix (Illustrative)**

| Factor | Low (+1) | Medium (+3) | High (+5) |
|---|---|---|---|
| Customer type | Resident salaried individual | Resident SME | Non-resident complex entity, trust |
| Geography (nationality/operations) | Domestic | Other listed transparent jurisdiction | High-risk / non-cooperative jurisdiction |
| Product mix | TD only, AMaturity | TD + foreign currency | TD + cross-border + cash-funded |
| Channel | Branch with full ID | Digital remote | Introduced via third party |
| Behaviour | Predictable | Mildly variable | Atypical, structured, layered |

Aggregate score determines the rating: **Low (5–8)**, **Medium (9–14)**, **High (15+)**. EDD is triggered at High; PEP status forces High regardless of score. Periodic refresh cadence: Low — every five (5) years; Medium — every three (3) years; High — annual. Trigger-based refresh applies upon material change in any factor.

## 3.6 FATCA / CRS Tax Residency Capture

A self-certification of tax residency shall be obtained from every customer (and, where applicable, every controlling person), capturing all jurisdictions of tax residency and the corresponding tax identification numbers. The certification shall be validated for plausibility against KYC data; inconsistencies (e.g., a stated US person without a US TIN) shall be queried before opening. Annual reporting obligations under FATCA and CRS are addressed in Chapter 9. **[Jurisdiction-Dependent]** Implementation reflects the local transposition of these international frameworks.

## 3.7 Onboarding Red Flags and Decline / Exit Procedures

Officers shall be alert to the following onboarding **[Red Flags]**: reluctance to provide standard ID; mismatched documents; unexplained third-party funding; requests for unusual confidentiality; pressure to expedite outside cut-off; ID documents from jurisdictions inconsistent with stated residence; round-sum cash deposits that approach but do not exceed reporting thresholds (structuring); use of intermediaries with no clear economic rationale; nominees and front-persons.

Where onboarding is declined, the decision and reasoning shall be recorded; the customer shall be informed politely and without disclosing internal control logic. Where an existing relationship must be exited (de-risked), SOP-017 governs the orderly closure.

### Standard Operating Practices in this Chapter

---

**SOP-010 — Individual Customer Onboarding and ID Verification**
- **Purpose:** Establish identity of a natural-person depositor to the Bank's standard.
- **Trigger:** New customer application.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager for high-risk.
- **Inputs:** Government-issued photographic ID; address verification document; KYC questionnaire; tax self-certification.
- **Procedure:**
  1. Officer requests primary and secondary documents.
  2. Officer verifies the documents against issuing-authority data sources where available.
  3. Biometric or in-person verification is completed.
  4. KYC questionnaire is captured in the system; risk rating is computed.
  5. Screening (sanctions, PEP, adverse media) is run; hits are routed to Financial Crime.
  6. Customer file is opened upon clearance.
- **Controls:** Four-eyes on every individual onboarding; system blocks deposit booking against an unverified customer record. **[Control Point]**
- **Evidence:** Document images; checklist; screening result; risk rating record. **[Audit Evidence]**
- **Reference:** Customer Acceptance Policy.

---

**SOP-011 — Corporate / Trust / Partnership Onboarding and Mandate Capture**
- **Purpose:** Onboard non-natural-person customers with full ownership and authority transparency.
- **Trigger:** New corporate/trust/partnership application.
- **Roles:** Maker — Corporate Service Officer; Checker — Compliance Officer; Approver — Head of Corporate Onboarding.
- **Inputs:** Certificate of incorporation / trust deed / partnership deed; constitutional documents; UBO declaration; authorised signatory list; corporate resolution authorising the relationship.
- **Procedure:**
  1. Officer collects and verifies constitutional documents through the relevant registry.
  2. UBOs identified down to natural-person level; each UBO is subject to SOP-010 procedures.
  3. Authorised signatories are captured with specimen signatures and combination rules (e.g., any two of three).
  4. Corporate resolution authorising the time deposit relationship is filed.
  5. Sanctions and PEP screening is run on the entity, UBOs, directors, and signatories.
- **Controls:** Annual review of corporate KYC; signatory updates require fresh resolution. **[Control Point]**
- **Evidence:** Constitutional documents; UBO declaration; signatory mandate; resolution. **[Audit Evidence]**
- **Reference:** Customer Acceptance Policy.

---

**SOP-012 — Joint, Minor, and Power-of-Attorney Account Onboarding**
- **Purpose:** Govern accounts with non-standard signing or capacity arrangements.
- **Trigger:** Application involving joint holders, a minor depositor, or operation by an attorney.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager.
- **Inputs:** ID of all holders; birth certificate for minors; appointment of guardian where required; original power of attorney with legal verification.
- **Procedure:**
  1. For joint holders, the operating mandate (either/survivor; jointly; jointly or survivor) is captured.
  2. For minors, the guardian is identified; the operating capacity ceases upon majority and is reviewed.
  3. For PoA, legal verifies the instrument; the scope of authority is recorded.
  4. Special instructions (in case of demise of one holder, etc.) are documented.
- **Controls:** All PoAs reviewed annually; any reported revocation is processed within twenty-four (24) hours. **[Control Point]**
- **Evidence:** Mandate; PoA instrument; legal opinion where applicable. **[Audit Evidence]**
- **Reference:** Customer Acceptance Policy; local Capacity Law. **[Jurisdiction-Dependent]**

---

**SOP-013 — PEP and Sanctions Screening, Hit Clearance, and L2/L3 Escalation**
- **Purpose:** Detect and treat exposure to PEPs and sanctioned parties.
- **Trigger:** Onboarding; periodic re-screening; ad hoc upon list update.
- **Roles:** Maker — Onboarding Officer; Checker — Financial Crime Analyst (L1); Approver — Senior Financial Crime Officer (L2) / MLRO (L3).
- **Inputs:** Customer data; consolidated sanctions and PEP lists; adverse-media feed.
- **Procedure:**
  1. Screening engine runs at onboarding and at every list update.
  2. Possible matches are routed to L1 for triage.
  3. False positives are cleared with documented reasoning.
  4. Confirmed PEPs proceed only with senior approval and EDD; confirmed sanctions matches are blocked and reported.
  5. The MLRO (Money Laundering Reporting Officer) is informed of every confirmed PEP onboarded.
- **Controls:** Quarterly QA sample on cleared hits; daily ageing of unresolved hits. **[Control Point]**
- **Evidence:** Screening log; clearance reasoning; approval record. **[Audit Evidence]**
- **Reference:** Financial Crime Policy. **[Jurisdiction-Dependent]**

---

**SOP-014 — Enhanced Due Diligence (EDD) for High-Risk Customers**
- **Purpose:** Apply commensurate depth of investigation to elevated-risk relationships.
- **Trigger:** High risk rating; PEP status; high-risk geography; large or complex deposit.
- **Roles:** Maker — Senior Onboarding Officer; Checker — Financial Crime Officer; Approver — MLRO.
- **Inputs:** Source-of-funds and source-of-wealth evidence; reputational due diligence; intended account activity profile.
- **Procedure:**
  1. Officer collects and reviews SoF/SoW evidence to corroborate self-declaration.
  2. Reputational research is performed using approved subscriptions.
  3. The expected activity profile (deposit volume, tenor, frequency, sources, beneficiaries) is recorded.
  4. The EDD pack is approved by the MLRO; the approval is time-limited.
  5. Ongoing transaction monitoring is calibrated against the activity profile.
- **Controls:** EDD packs reviewed annually; deviations from expected activity profile trigger transaction monitoring alerts. **[Control Point]**
- **Evidence:** EDD pack; MLRO approval; activity profile. **[Audit Evidence]**
- **Reference:** Financial Crime Policy.

---

**SOP-015 — FATCA/CRS Self-Certification Capture and Validation**
- **Purpose:** Collect, validate, and retain tax residency information for international information-exchange reporting.
- **Trigger:** Onboarding; change in circumstances; periodic refresh.
- **Roles:** Maker — Onboarding Officer; Checker — Tax Operations Analyst; Approver — Head of Tax Operations.
- **Inputs:** Self-certification form; KYC particulars.
- **Procedure:**
  1. Officer obtains the customer's signed self-certification, listing every jurisdiction of tax residency and corresponding TIN.
  2. Tax Operations validates plausibility against KYC; e.g., US-place-of-birth without a US TIN triggers cure-letter procedure.
  3. Records are tagged for the relevant reporting year.
  4. Customers are obliged to inform the Bank of changes; failure to recertify within ninety (90) days of an identified change-in-circumstance results in reportable-by-default treatment.
- **Controls:** Annual quality check on a stratified sample; pre-reporting validation. **[Control Point]**
- **Evidence:** Signed self-certification; cure-letter trail. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Local transposition of FATCA and the CRS Common Reporting Standard.

---

**SOP-016 — Periodic KYC Refresh by Risk Tier**
- **Purpose:** Maintain KYC currency over the life of the relationship.
- **Trigger:** Refresh due-date; event trigger (change of address, change of UBO).
- **Roles:** Maker — Relationship Officer or RM; Checker — Compliance Analyst; Approver — Compliance Manager for High-risk refreshes.
- **Inputs:** Latest customer documents; updated screening; updated activity profile.
- **Procedure:**
  1. The system queues refresh tasks ahead of due-date.
  2. Officer contacts the customer; collects updated documents.
  3. Compliance reviews and re-rates.
  4. Where refresh is not completed by due-date plus a defined grace period, the account is restricted from new transactions.
- **Controls:** Refresh due-date dashboard reviewed monthly; aged overdue refreshes escalate to the Operating Risk Committee. **[Control Point]**
- **Evidence:** Refresh task closure; updated KYC pack. **[Audit Evidence]**
- **Reference:** Financial Crime Policy.

---

**SOP-017 — Customer Exit and De-Risking Decision**
- **Purpose:** Manage the orderly exit of customers whose continued banking is incompatible with the Bank's risk appetite.
- **Trigger:** Compliance recommendation to exit; sanctions hit confirmation; KYC refresh failure; protracted unsatisfactory activity.
- **Roles:** Maker — Compliance Officer; Checker — MLRO; Approver — Exit Committee.
- **Inputs:** Compliance case file; customer-relationship history.
- **Procedure:**
  1. The case is brought to the Exit Committee with a written recommendation.
  2. Upon approval, the customer is given written notice of the Bank's intention to close the relationship, with a notice period consistent with contractual and consumer-protection obligations.
  3. Time deposits in flight are run off to maturity unless held under a sanctions block, in which case statutory blocking governs.
  4. Funds are released to the customer per their instruction, subject to AML and tax clearance.
  5. The customer's particulars are tagged so that re-entry is flagged.
- **Controls:** Quarterly exit committee review of pending and completed exits. **[Control Point]**
- **Evidence:** Exit case file; notice letter; closure records. **[Audit Evidence]**
- **Reference:** Customer Exit Policy. **[Jurisdiction-Dependent]**

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 4 — Account Opening, Funding & Certificate Issuance

## 4.1 Application Form, Mandate, and Specimen Signatures

The Bank accepts time deposits only on the strength of a completed, signed application form bearing all material particulars: customer identifier, principal sum and currency, product code and tenor, interest payment frequency, maturity instruction, fee acknowledgement, and the customer's signature. Where the deposit is opened via a digital channel, the equivalent particulars shall be captured in a digital flow with an audited acceptance step. The specimen signature (or its digital equivalent) shall be on file before booking. The mandate shall be reviewed before any servicing instruction is acted upon (Chapters 6 and 7).

## 4.2 Funding Channels: Cash, Internal Transfer, Inward Remittance, Cheque

Funding may be received through any of the following channels: cash at the branch counter (subject to cash transaction reporting thresholds), debit of an existing account held with the Bank, inward wire transfer, or cheque deposit. The cleared-funds rule is universal: no time deposit shall be activated against uncleared funds. For cheque funding, the deposit is held in a clearing-suspense state and activated only upon clearance; the contractual start-date for accrual purposes is then explicitly disclosed to the customer.

## 4.3 Value-Dating Rules and Cut-Off Times

Each branch publishes its cut-off times for same-day value-dating. Transactions submitted after cut-off are value-dated the next business day. The accrual engine values from (and including) the value date; the maturity date is computed by tenor advancement against the value date and subject to business-day conventions (modified following, by default), with weekend and public-holiday treatment defined in section 5.3 and Chart of Accounts disclosures.

## 4.4 TD Certificate / Advice Issuance (Physical vs Digital)

Upon successful booking, the Bank shall issue to the depositor a deposit confirmation that, depending on the channel, takes the form of (a) a physical Certificate of Deposit, (b) a printed advice, or (c) a digital advice retrievable from the customer's digital banking record. The confirmation shall be a non-negotiable acknowledgement and shall bear the deposit reference, particulars, and the disclosed terms. Physical certificates are issued from a controlled series, the inventory of which is reconciled monthly.

## 4.5 Nominee, Beneficiary, and Maturity Instruction Capture

At booking, the customer's instructions shall be captured for: (a) maturity action — *renew principal only / renew principal + interest / credit to designated account / pay by manager's cheque*; (b) interim interest payment route, where applicable; (c) nominee or beneficiary, where the product or jurisdiction supports nomination. Default instructions shall not be applied without an explicit customer choice; pre-ticked boxes are prohibited.

## 4.6 Maker-Checker on Account Creation in Core Banking

Every booking in the core banking system shall be subject to maker-checker separation. The Officer enters the booking; the Checker independently verifies the principal, tenor, rate, maturity date, customer reference, and the funding source against the application and the funding evidence. Only upon Checker approval is the deposit activated and the certificate generated.

### Standard Operating Practices in this Chapter

---

**SOP-018 — Application Intake, Completeness Check, and Maker-Checker Booking**
- **Purpose:** Convert a customer's instruction into a booked deposit with full control.
- **Trigger:** Signed application received.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager for amounts above threshold.
- **Inputs:** Signed application; KFS reference; funding evidence; KYC clearance.
- **Procedure:**
  1. Officer checks completeness of the application; missing particulars are clarified before submission.
  2. Officer keys the booking in CBS; the maker entry remains pending.
  3. Checker independently verifies the seven core fields: customer, principal, currency, product, tenor, rate, maturity instruction.
  4. Approver releases for amounts above branch threshold.
  5. CBS activates the deposit and triggers certificate generation.
- **Controls:** Daily maker-checker exception report; standing rule that no Officer may check own work. **[Control Point]**
- **Evidence:** CBS audit trail; signed application. **[Audit Evidence]**
- **Reference:** Branch Operations Manual.

---

**SOP-019 — Funding Verification by Channel and Cleared-Funds Rule**
- **Purpose:** Ensure the deposit is funded with good funds before activation.
- **Trigger:** Booking pending funding confirmation.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager.
- **Inputs:** Funding source evidence (debit confirmation, cash receipt, cheque clearance, wire MT103, etc.).
- **Procedure:**
  1. For internal debits: confirm sufficient balance; place the lien; debit and credit the booking suspense.
  2. For cash: confirm count by dual-control; issue receipt; observe CTR thresholds.
  3. For cheque: hold in suspense pending clearance per the cheque clearing calendar.
  4. For inward wire: match by reference; confirm originator details for AML.
  5. Activate the deposit only upon confirmed cleared funds.
- **Controls:** End-of-day reconciliation of booking-suspense to funding evidence. **[Control Point]**
- **Evidence:** Funding evidence; suspense aging report. **[Audit Evidence]**
- **Reference:** Cash and Clearing Operations Manual.

---

**SOP-020 — Cash Deposit Handling for TD Funding (CTR Thresholds)**
- **Purpose:** Govern cash funding with respect to safety, AML, and reporting.
- **Trigger:** Customer presents cash to fund a deposit.
- **Roles:** Maker — Teller; Checker — Head Teller; Approver — Branch Manager for amounts above a threshold.
- **Inputs:** Cash; customer identification; declaration where required.
- **Procedure:**
  1. Teller verifies authenticity of notes using detection equipment.
  2. Counts under dual-control; CCTV coverage maintained.
  3. Cash transaction report is generated for amounts at or above the **[Jurisdiction-Dependent]** CTR threshold.
  4. The customer's declared source of funds is recorded; **[Red Flag]** structuring patterns (e.g., two deposits just below the threshold within a short period) are escalated to Financial Crime.
- **Controls:** End-of-day cash reconciliation; weekly CTR completeness check. **[Control Point]**
- **Evidence:** CTR submission; CCTV reference; declaration. **[Audit Evidence]**
- **Reference:** Cash Operations Manual.

---

**SOP-021 — TD Certificate / E-Advice Generation, Dispatch, and Acknowledgement**
- **Purpose:** Issue, dispatch, and confirm receipt of the customer's deposit confirmation.
- **Trigger:** Deposit activated in CBS.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Operations Controller for series reconciliation.
- **Inputs:** Activated deposit record; certificate template; series inventory (physical certificates).
- **Procedure:**
  1. CBS generates the certificate or advice from the controlled template.
  2. For physical certificates, the Officer draws from the series register; both the issued and the spoilt forms are recorded against the series.
  3. Customer signs the receipt acknowledgement.
  4. Digital advices are pushed to the customer's digital banking inbox; opening and download events are logged.
- **Controls:** Monthly reconciliation of series inventory to issued/spoilt certificates. **[Control Point]**
- **Evidence:** Series register; signed acknowledgement; digital advice audit trail. **[Audit Evidence]**
- **Reference:** Stationery Control Policy.

---

**SOP-022 — Capture of Maturity Instruction (Rollover/Redeem) and Nominee Details**
- **Purpose:** Ensure post-maturity treatment matches the customer's wishes.
- **Trigger:** Booking; subsequent amendment.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager.
- **Inputs:** Customer instruction; nominee form where applicable.
- **Procedure:**
  1. Officer presents the maturity options and records the customer's choice with explicit, dated consent.
  2. Where applicable, the nominee form is collected, signed, and witnessed.
  3. The maturity instruction is keyed in CBS; an amendment requires SOP-032.
  4. The customer receives a confirmation of the maturity instruction by their preferred channel.
- **Controls:** Pre-maturity reports cross-check the instruction on file. **[Control Point]**
- **Evidence:** Customer instruction; nominee form; CBS instruction trail. **[Audit Evidence]**
- **Reference:** Branch Operations Manual.

---

**SOP-023 — Same-Day Cancellation / Cooling-Off Handling**
- **Purpose:** Process customer cancellation requests within the cooling-off window where granted by product or law.
- **Trigger:** Customer requests cancellation within the cooling-off period.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager.
- **Inputs:** Original application; customer request.
- **Procedure:**
  1. Officer verifies that the request falls within the documented cooling-off window.
  2. CBS booking is reversed; principal returned to source; no interest accrues for the day(s) the funds were held, unless product terms specify otherwise.
  3. Certificate is recovered or marked cancelled; series register is updated.
  4. The cancellation is logged for product MIS.
- **Controls:** Daily cooling-off cancellation report; trend monitoring for mis-selling indicators. **[Control Point]**
- **Evidence:** Customer cancellation request; CBS reversal trail. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Consumer Protection regulation.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 5 — Interest Accrual, Capitalisation & Day-Count Conventions

## 5.1 Day-Count Conventions

The amount of interest accrued in a period is the product of the principal, the annualised rate, and a time fraction. The numerator and denominator of that time fraction are determined by the day-count convention, of which the Bank uses four:

- **30/360 (Bond Basis):** Each month is deemed to be 30 days; the year is deemed to be 360 days. Used historically for fixed-income instruments and certain corporate deposits.
- **ACT/360 (Money Market):** Actual calendar days in the period over a 360-day year. Standard for most USD, EUR, and CHF money-market deposits.
- **ACT/365 Fixed:** Actual days over a fixed 365-day year. Standard for many GBP, HKD, and SGD deposits and frequently used for retail customer disclosures.
- **ACT/ACT:** Actual days over actual days in the year (366 in leap years). Used for certain government and longer-dated instruments.

The convention applied to each product is fixed in the Product Programme Document and reflected in the KFS.

> **Worked Example — Interest on USD 100,000.00 @ 5.00% p.a. for 90 days:**
>
> - 30/360: 100,000 × 5.00% × (90/360) = **USD 1,250.00**
> - ACT/360: 100,000 × 5.00% × (90/360) = **USD 1,250.00**
> - ACT/365 Fixed: 100,000 × 5.00% × (90/365) = **USD 1,232.88**
> - ACT/ACT (non-leap): 100,000 × 5.00% × (90/365) = **USD 1,232.88**

Even small differences accumulate; consistency between booking, accrual, advice, and certificate is a control concern.

## 5.2 Simple versus Compound Interest

The Bank's default for time deposits is **simple interest** when interest is paid at maturity in a single tranche. **Compound interest** applies where the product permits or requires capitalisation of interest at sub-periods (monthly, quarterly, semi-annually) during the tenor.

- Simple interest: *I = P × r × (t / B)*
- Compound interest: *A = P × (1 + r/n)^(n × t)*

Where *P* = principal, *r* = nominal annual rate, *t* = time in years, *B* = day-count basis, *n* = compounding frequency per annum, *A* = accumulated amount.

> **Worked Example — Effective Annual Rate (EAR):** A 4.00% p.a. nominal rate compounded monthly equates to *EAR = (1 + 0.04/12)^12 − 1 ≈ 4.07%*.

The KFS shall disclose both nominal and effective rates whenever compounding is offered.

## 5.3 Accrual Engine: Daily Run, Holiday/Weekend Handling

The accrual engine processes daily, generating an accrual entry per live deposit in the subledger. Weekend and public-holiday days are accrued forward on the next business day (i.e., interest still accrues over those days, but the accounting entry is dated to the next business day, with the value-date showing the calendar day(s) accrued). End-of-month, end-of-quarter, and end-of-year are landmark dates and shall be reconciled separately under SOP-028.

The maturity date is computed under the modified following business-day convention by default: if the contractual maturity date falls on a non-business day, the deposit matures on the next business day, unless that next business day falls in the next month, in which case it matures on the previous business day. Accrual continues through the adjusted maturity date.

## 5.4 Interest Payment Modes

Permitted modes are: (a) **At maturity** — interest paid in a single tranche together with the principal; (b) **Periodic (monthly, quarterly, semi-annually)** — interest paid into a designated current or savings account on the scheduled dates; (c) **Capitalised** — interest is added to the principal at the schedule date and accrues thereafter on the higher base.

## 5.5 GL Postings for Accrual and Payment

Interest accrual and payment generate the following standard journal entries. Account codes are illustrative and shall be replaced by the Bank's Chart of Accounts:

> **Funding at Inception**
> ```
> Dr  1010-CASH-BRANCH                    USD 100,000.00
>    Cr  2210-TD-PRINCIPAL-CUST                USD 100,000.00
> Narrative: Funding of TD #TD-2026-000123, 12M, 4.25% p.a.
> ```
>
> **Daily Accrual**
> ```
> Dr  8110-INT-EXP-TD                     USD     11.64
>    Cr  2215-TD-INT-PAYABLE                    USD     11.64
> Narrative: Daily accrual TD #TD-2026-000123, ACT/365, 1 day
> ```
>
> **Periodic Interest Payment (with Withholding Tax)**
> ```
> Dr  2215-TD-INT-PAYABLE                 USD  1,062.50
>    Cr  1110-CASA-CUST                         USD    902.13
>    Cr  2270-WHT-PAYABLE                       USD    159.38
>            (assuming illustrative 15% WHT on resident interest)
> Narrative: Quarterly interest credit TD #TD-2026-000123
> ```
>
> **Capitalisation at Sub-Period (for rollover at maturity)**
> ```
> Dr  2215-TD-INT-PAYABLE                 USD  1,062.50
>    Cr  2210-TD-PRINCIPAL-CUST                USD  1,062.50
> Narrative: Capitalisation TD #TD-2026-000123
> ```
>
> **Maturity Redemption to Customer Current Account**
> ```
> Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
> Dr  2215-TD-INT-PAYABLE                 USD  4,250.00
>    Cr  1110-CASA-CUST                         USD 104,250.00
> Narrative: Maturity payout TD #TD-2026-000123
> ```

## 5.6 Withholding Tax at Source and Net-of-Tax Crediting

Where the prevailing law requires withholding tax on interest paid to depositors, the WHT shall be computed at the point of interest payment (or capitalisation), deducted from the gross interest, and credited to the WHT Payable GL pending statutory remittance. **[Jurisdiction-Dependent]** Rates differ by residency status, by treaty entitlement, and by exempt status (e.g., charities); the Tax Operations team maintains the WHT matrix.

## 5.7 Recalculation, Back-Value, and Adjustment Controls

Errors discovered post-posting are corrected via back-value adjustment under SOP-027. Back-value adjustments shall not be used to alter interest in favour of a counterparty or to disguise booking errors; any adjustment exceeding the materiality threshold shall be reported to the Operating Risk Committee.

### Standard Operating Practices in this Chapter

---

**SOP-024 — End-of-Day Interest Accrual Run and Exception Review**
- **Purpose:** Compute and post daily interest accruals across the time deposit book.
- **Trigger:** End-of-day batch schedule.
- **Roles:** Maker — Operations Batch Officer; Checker — Operations Controller; Approver — Head of Finance Operations on exception closure.
- **Inputs:** Live deposit subledger; rate table; day-count configuration; calendar.
- **Procedure:**
  1. The accrual job runs after the daily end-of-business cutover.
  2. The exception report lists deposits skipped (e.g., due to data issues, zero balance, rate-table mismatch).
  3. Exceptions are investigated and cleared before the next-day book opens.
  4. The total accrual posted is reconciled to expected value, computed as a control total at the product-and-currency level.
- **Controls:** No book may open the next day with an unresolved accrual exception; ageing of unresolved exceptions reported daily. **[Control Point]**
- **Evidence:** Batch log; exception report; reconciliation evidence. **[Audit Evidence]**
- **Reference:** End-of-Day Operations Manual.

---

**SOP-025 — Periodic Interest Payment to Customer Account and GL Posting**
- **Purpose:** Pay scheduled interest correctly and on time.
- **Trigger:** Scheduled interest payment date for products with periodic payment.
- **Roles:** Maker — Operations Batch Officer; Checker — Operations Controller.
- **Inputs:** Interest payment schedule; customer account standing instructions.
- **Procedure:**
  1. CBS schedules each periodic interest payment by deposit.
  2. The batch debits the interest payable, deducts WHT where applicable, and credits the designated customer account.
  3. Failed credits (closed account, frozen account) are routed to a payment-suspense for follow-up within two (2) business days.
  4. Customer advice is generated.
- **Controls:** Daily payment-suspense aging report; zero-tolerance for aged items beyond five (5) business days. **[Control Point]**
- **Evidence:** Payment batch log; customer advices; suspense register. **[Audit Evidence]**
- **Reference:** Interest Payment Procedures.

---

**SOP-026 — Withholding Tax Computation, Deduction, and Tax-GL Sweep**
- **Purpose:** Discharge the Bank's obligation as withholding agent.
- **Trigger:** Interest payment or capitalisation event.
- **Roles:** Maker — Tax Operations Analyst; Checker — Finance Controller; Approver — Head of Tax Operations.
- **Inputs:** WHT matrix; customer residency/exemption status; treaty documentation.
- **Procedure:**
  1. CBS applies the WHT rate by reference to the customer's status and the prevailing matrix.
  2. The deducted amount is posted to the WHT Payable GL.
  3. Treaty-relief and exemption cases are flagged for additional review and supported by documentation on file.
  4. The Bank remits the WHT to the tax authority by the statutory deadline (SOP-047).
- **Controls:** Monthly reconciliation of WHT GL to underlying interest event log; sample review on treaty-relief cases. **[Control Point]**
- **Evidence:** WHT calculation log; treaty documents. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Tax law and treaty network.

---

**SOP-027 — Back-Value Adjustment and Interest Recomputation**
- **Purpose:** Correct dated errors discovered after the event without distorting the audit trail.
- **Trigger:** Error in tenor, rate, day-count, or principal identified after accrual has commenced.
- **Roles:** Maker — Branch Officer or Operations Officer; Checker — Operations Controller; Approver — Head of Finance Operations.
- **Inputs:** Root-cause analysis; corrected accrual computation; customer-impact statement.
- **Procedure:**
  1. The originator submits the back-value request with supporting evidence.
  2. Operations recomputes the accrual from the original value date to the date of correction.
  3. Reversal and re-booking entries are posted with the back-value flag; the customer is informed where their net position changes.
  4. The case is logged in the operational incident register.
- **Controls:** Threshold-based escalation to OpRisk Committee; quarterly trend review. **[Control Point]**
- **Evidence:** Adjustment request; GL entries; customer notification. **[Audit Evidence]**
- **Reference:** Operational Incident Policy.

---

**SOP-028 — Accrual Reconciliation: Subledger versus General Ledger**
- **Purpose:** Confirm completeness and accuracy of accrual postings.
- **Trigger:** End-of-day; period-end.
- **Roles:** Maker — Reconciler; Checker — Finance Manager; Approver — Head of Finance Operations.
- **Inputs:** Subledger accrual report; GL balance for interest expense and interest payable.
- **Procedure:**
  1. Reconciler extracts the day's accrual at product-and-currency level from the subledger.
  2. Reconciler matches to the GL postings; differences are itemised by deposit.
  3. Differences are aged; ageing beyond two (2) business days triggers escalation.
  4. Period-end reconciliations are signed off and retained as part of the financial close.
- **Controls:** Independent of the accrual maker; reconciliation breaks dashboard reviewed daily. **[Control Point]**
- **Evidence:** Reconciliation file; sign-off. **[Audit Evidence]**
- **Reference:** Reconciliation Policy.

---

**SOP-029 — Holiday/Weekend Rollforward and Value-Date Correction**
- **Purpose:** Apply business-day conventions correctly across weekends, public holidays, and currency holidays.
- **Trigger:** Booking; maturity date computation; FCY deposit involving a non-domestic holiday.
- **Roles:** Maker — Branch Officer or CBS calendar administrator; Checker — Operations Controller.
- **Inputs:** Domestic and currency holiday calendars; product business-day convention.
- **Procedure:**
  1. The CBS calendar table is updated annually and ad hoc upon new statutory holidays.
  2. Bookings on or with a maturity falling on a non-business day apply the modified-following convention by default; exceptions per product are configured.
  3. Where a currency holiday affects an FCY deposit, the maturity date is computed using the joint calendar.
  4. Misapplied conventions trigger back-value correction under SOP-027.
- **Controls:** Annual calendar review; pre-period-end review of upcoming holiday-spanning deposits. **[Control Point]**
- **Evidence:** Calendar configuration; pre-period reports. **[Audit Evidence]**
- **Reference:** Business-Day Convention Standard.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 6 — Rollover, Renewal & Mid-Term Events

## 6.1 Rollover Types

At maturity, a deposit may be rolled over in one of three contractually defined modes: (a) **Principal only** — interest paid out per the standing instruction; principal renewed for the same tenor at the prevailing rate; (b) **Principal plus interest** — the total of principal and accumulated net-of-tax interest renewed; (c) **Custom** — a different tenor, rate (where exception approved), or split renewal is applied per the customer's written instruction received before maturity.

## 6.2 Standing Instruction Capture and Amendment

The standing instruction is captured at inception under SOP-022. Amendments shall be received in writing, identified to the customer's specimen signature or digital authentication, and processed under SOP-032 with a deadline of no later than one (1) business day before maturity, to allow Treasury Operations to apply funding cover.

## 6.3 Grace Period and Treatment of Lapsed Instructions

Where the customer has not provided a maturity instruction, the default treatment defined in the product PPD applies. The Bank's default for retail products is to renew principal only at the prevailing rate; the alternative (no renewal, with maturity proceeds placed in a non-interest-bearing matured-deposits account) is reserved for products and segments where that practice is consistent with consumer-protection norms. The default treatment shall be displayed on the KFS and the certificate.

## 6.4 Mid-Term Top-Up and Partial Withdrawal

Mid-term top-up (increasing principal during the tenor) is not permitted on most conventional time deposit products and shall be processed only where the PPD explicitly allows. Where allowed, the top-up amount accrues at either the original rate (continuation product) or the prevailing rate for the remaining tenor (residual-tenor product); the methodology is defined per product.

Partial withdrawal mid-tenor is permitted only on products that explicitly support it; the methodology for break-cost on the withdrawn portion is set out in Chapter 7.

## 6.5 Customer Notification: Pre-Maturity Advice

The Bank shall send the customer a pre-maturity advice at T-7 (seven business days before maturity) and a reminder at T-3, reflecting the current standing instruction. The reminder enables the customer to amend the instruction before cut-off, restate maturity destination, or arrange logistics for proceeds. Where the deposit is in a foreign currency, the advice shall remind the customer of any FX conversion that will result.

### Standard Operating Practices in this Chapter

---

**SOP-030 — Pre-Maturity Notification (T-7 / T-3) and Instruction Confirmation**
- **Purpose:** Give the depositor an informed window to confirm or amend the maturity instruction.
- **Trigger:** Standing schedule at T-7 and T-3 prior to each maturity.
- **Roles:** Maker — CBS automated notification; Checker — Operations Officer reviews exceptions.
- **Inputs:** Maturity calendar; standing instruction; customer contact preference.
- **Procedure:**
  1. CBS generates and dispatches advices via customer's preferred channel.
  2. Delivery failures are queued for branch follow-up.
  3. Customer responses (amendments) are routed to SOP-032.
- **Controls:** Daily delivery-success report; exception follow-up within two (2) business days. **[Control Point]**
- **Evidence:** Advice dispatch log; amendment audit trail. **[Audit Evidence]**
- **Reference:** Customer Communications Standard.

---

**SOP-031 — Automatic Rollover Processing and Rate-on-Renewal Application**
- **Purpose:** Renew principal (and, where instructed, interest) at maturity at the prevailing rate.
- **Trigger:** Maturity date for deposits with a standing renewal instruction.
- **Roles:** Maker — CBS batch; Checker — Operations Controller.
- **Inputs:** Rate sheet effective on the maturity date; standing instruction; tax treatment.
- **Procedure:**
  1. At end-of-day on maturity, the deposit is closed and a new deposit is opened with the same reference family (e.g., parent-child linkage retained for audit).
  2. The prevailing rate for the matching tenor and customer segment is applied unless an exception is on file.
  3. Interest is paid out, capitalised, or rolled depending on instruction.
  4. A new certificate or advice is issued.
- **Controls:** Daily renewal pricing audit by Treasury Risk; exception flag where the applied rate is below the floor or above the ceiling configured. **[Control Point]**
- **Evidence:** CBS renewal trail; new advice; rate audit log. **[Audit Evidence]**
- **Reference:** Rollover Procedures.

---

**SOP-032 — Amendment of Standing Maturity Instruction**
- **Purpose:** Process changes to the maturity instruction with appropriate verification.
- **Trigger:** Customer request to amend prior to maturity.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager.
- **Inputs:** Customer written instruction with specimen or digital signature; identification verification.
- **Procedure:**
  1. Officer verifies the customer's identity and the genuineness of the instruction.
  2. The amendment is keyed in CBS and routed for checker release.
  3. The amendment is confirmed back to the customer by a separate channel where the change is material (e.g., destination account changed).
  4. Amendments received later than one (1) business day before maturity may not be effected and the customer is informed.
- **Controls:** Out-of-band callback for material amendments; **[Red Flag]** monitoring for amendments shortly after onboarding or shortly before redemption. **[Control Point]**
- **Evidence:** Customer instruction; CBS amendment trail; callback log. **[Audit Evidence]**
- **Reference:** Anti-Fraud Standard.

---

**SOP-033 — Partial Withdrawal Processing Where Product Permits**
- **Purpose:** Execute partial withdrawals on products that contractually allow them.
- **Trigger:** Customer request; product feature enabled.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Operations Controller for amounts above the branch threshold.
- **Inputs:** PPD feature flag; customer request; break-cost computation.
- **Procedure:**
  1. Officer verifies the customer's identity and product eligibility.
  2. The break-cost on the withdrawn portion is computed under SOP-035 and disclosed to the customer.
  3. Upon customer confirmation, the partial closure is booked: the principal is reduced; the corresponding interest and any break-cost are applied; the deposit continues on the residual principal.
  4. A revised certificate/advice is issued.
- **Controls:** Pre-disclosure of break-cost and customer acknowledgement before booking. **[Control Point]**
- **Evidence:** Customer acknowledgement; CBS partial-closure trail. **[Audit Evidence]**
- **Reference:** Break-Cost Standard.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 7 — Early Withdrawal, Break Costs & Maturity Redemption

## 7.1 Eligibility for Early Withdrawal and Customer Request Channels

Early withdrawal is permitted only where the product feature is enabled in the PPD and disclosed on the KFS. Where the feature is enabled, the Bank may, in its discretion, accept the customer's request, normally subject to a minimum elapsed tenor (e.g., seven days) and to the application of a break cost. The customer may request early withdrawal in person at the branch, via authenticated digital channels where supported, or in writing to the customer service team.

## 7.2 Break-Cost / Early Withdrawal Penalty Formulae

The Bank applies one of two break-cost methodologies, as specified in the PPD:

**(a) Interest-Forfeiture Method (default retail):**

> *Penalty = Accrued or paid interest on the broken portion × Forfeiture %*
>
> Forfeiture % is tiered against elapsed tenor:
> - Less than 25% of tenor elapsed: 100% forfeiture
> - 25% – 50% elapsed: 75% forfeiture
> - 50% – 75% elapsed: 50% forfeiture
> - 75% – 100% elapsed: 25% forfeiture
>
> (Illustrative tiers; actual tiers are set per product.)
>
> Net interest paid to the customer = Interest computed at the contractual rate − Penalty.

**(b) Reinvestment-Loss Method (wholesale/institutional):**

> *Penalty = max(0, P × (r_contract − r_prevailing,remaining) × (Days_remaining / B))*
>
> where *r_prevailing,remaining* is the Bank's offered rate at the date of break for the residual tenor. Where *r_prevailing,remaining* exceeds *r_contract*, the Bank does not pay the difference to the customer (the floor at zero applies).

> **Worked Example (Interest-Forfeiture, Retail):**
>
> USD 100,000.00 placed on 12-month TD at 4.25% p.a., ACT/365. Customer requests break after 200 days (≈55% of tenor elapsed, 50% tier applies in illustration).
>
> - Interest computed at contractual rate: 100,000 × 4.25% × (200/365) = USD 2,328.77
> - Forfeiture at 50%: 2,328.77 × 50% = USD 1,164.38
> - Net interest paid: 2,328.77 − 1,164.38 = USD 1,164.38 (before WHT, if any)
> - Total payout: 100,000.00 + 1,164.38 (less WHT) = USD 101,164.38 less WHT.

## 7.3 Hardship Waivers and Compassionate Closure

The Bank may, in clearly documented hardship cases (terminal illness, death of the depositor, declared natural disaster, court order), waive all or part of the break cost. Hardship waivers shall be approved at the level set out in the Delegations of Authority and shall be subject to **[Audit Evidence]** retention. Hardship discretion shall not be exercised to facilitate operational error correction (use SOP-027) or to circumvent product rules.

## 7.4 Maturity Redemption: Payout Channels and Cleared-Funds

At maturity (and at acceptance of an early-withdrawal request), the principal and the net interest are paid through the customer's designated channel: credit to a current/savings account held with the Bank, manager's cheque, outward wire, or, where the customer presents in person and product allows, in cash subject to AML and cash-handling rules. Maturity payouts in foreign currency are subject to FX conversion only on the customer's explicit instruction.

## 7.5 Deceased Customer Estate Settlement

Upon receipt of notice of the depositor's demise, the deposit is placed under a Deceased Estate flag in the CBS that prevents further transactions other than statutory ones. The Bank shall not act on instructions from the deceased's account after the date of demise. Settlement proceeds in accordance with the local law of succession and the documentation produced (death certificate, grant of probate or letters of administration, court order where the deposit is contested). Joint mandates of the type "either/survivor" pay out to the survivor upon production of the death certificate.

## 7.6 Lost Certificate, Indemnity, and Duplicate Issuance

Where a physical certificate is reported lost, stolen, or destroyed, the customer applies for a duplicate. The application is accompanied by an indemnity in the Bank's standard form, properly executed (and witnessed where required), and after a notice period during which the loss is recorded against the certificate series. The duplicate is marked "DUPLICATE" and bears a new series number with a cross-reference to the original.

## 7.7 GL Reversals on Premature Closure

Premature closure generates the following standard journal: the accrued interest payable is settled, the break-cost is recognised as interest expense reversal (or other income, per accounting policy), and the principal is paid out.

> **Premature Closure with Break-Cost (Illustrative)**
> ```
> Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
> Dr  2215-TD-INT-PAYABLE                 USD  2,328.77
>    Cr  1110-CASA-CUST                         USD 101,164.38
>    Cr  8120-INT-EXP-RECOVERED                  USD  1,164.39
> Narrative: Premature closure TD #TD-2026-000123 with break-cost @ 50% forfeiture
> ```

### Standard Operating Practices in this Chapter

---

**SOP-034 — Customer-Initiated Early Withdrawal: Intake and Authority Check**
- **Purpose:** Authenticate the request and verify product eligibility before processing a break.
- **Trigger:** Customer request for early withdrawal.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager.
- **Inputs:** Customer request; identification; mandate; PPD.
- **Procedure:**
  1. Officer authenticates the customer.
  2. Officer verifies that early withdrawal is permitted on the product.
  3. Officer verifies the mandate (for joint and corporate accounts).
  4. The Officer initiates the break workflow that triggers SOP-035.
- **Controls:** Out-of-band callback for non-face-to-face requests above the threshold; **[Red Flag]** monitoring for unusual break patterns. **[Control Point]**
- **Evidence:** Customer request; identification record; mandate. **[Audit Evidence]**
- **Reference:** Break-Cost Standard.

---

**SOP-035 — Break-Cost Computation, Approval, and Customer Disclosure**
- **Purpose:** Compute and disclose the break cost before the deposit is broken.
- **Trigger:** Authenticated customer request to break.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Operations Controller for non-standard cases.
- **Inputs:** Product methodology; rate at the date of break (for reinvestment method); elapsed-tenor data.
- **Procedure:**
  1. CBS computes the break cost using the methodology specified in the PPD.
  2. The Officer reviews the result for sensibility; non-standard methodology variants are routed to Operations.
  3. The figure is disclosed to the customer in writing, with a clear net-payout indication.
  4. The customer signs the acknowledgement before the break is executed.
- **Controls:** Pre-break customer acknowledgement; sample QA on accuracy. **[Control Point]**
- **Evidence:** Disclosure document; customer acknowledgement; CBS computation trail. **[Audit Evidence]**
- **Reference:** Break-Cost Standard.

---

**SOP-036 — Hardship/Compassionate Waiver Approval and Logging**
- **Purpose:** Process discretionary waivers of break cost on hardship grounds.
- **Trigger:** Hardship case identified and documented.
- **Roles:** Maker — Branch Manager or Relationship Manager; Checker — Compliance Officer; Approver — Head of Liabilities per Delegations of Authority.
- **Inputs:** Hardship evidence; customer request.
- **Procedure:**
  1. The case file is prepared with documentary evidence (medical, court order, death certificate, declaration).
  2. The Approver records the decision and the amount waived.
  3. The waiver is booked as a separate accounting line and reported in the monthly waiver register.
- **Controls:** Aggregate waivers reported monthly to OpRisk; sampling for misuse. **[Control Point]**
- **Evidence:** Hardship case file; approver record; waiver register entry. **[Audit Evidence]**
- **Reference:** Delegations of Authority; Operational Risk Framework.

---

**SOP-037 — Maturity Payout Processing and Customer Settlement**
- **Purpose:** Pay maturity proceeds to the customer per their instruction.
- **Trigger:** Maturity date (with non-renew instruction); acceptance of an early-withdrawal request.
- **Roles:** Maker — Operations Officer or Branch Officer; Checker — Operations Controller or Branch Service Manager.
- **Inputs:** Customer instruction; deposit record; payout channel particulars.
- **Procedure:**
  1. CBS computes the net payout (principal + net interest − any break cost − WHT).
  2. The payment instrument is generated per the customer's instruction.
  3. For outward wires, sanctions screening is run on the beneficiary.
  4. The deposit record is closed; the certificate is marked redeemed; the customer receives a final advice.
- **Controls:** Maturity payout suspense aging dashboard; nil-balance reconciliation. **[Control Point]**
- **Evidence:** Final advice; payment instrument; CBS closure trail. **[Audit Evidence]**
- **Reference:** Payments Procedures.

---

**SOP-038 — Deceased Estate Claim Handling and Disbursement**
- **Purpose:** Discharge the Bank's liability to the estate of a deceased depositor lawfully.
- **Trigger:** Notice of demise of the depositor.
- **Roles:** Maker — Estates Officer; Checker — Legal Officer; Approver — Head of Estates and Court Orders.
- **Inputs:** Death certificate; succession documents (probate, letters of administration, court order); identification of claimants.
- **Procedure:**
  1. CBS places the relationship under Deceased Estate flag immediately upon notice.
  2. Estates Officer collects the succession documents; Legal confirms sufficiency.
  3. For joint either-or-survivor accounts, the survivor is paid upon production of the death certificate; for sole accounts, payment is made to the legal personal representative.
  4. The settlement is recorded; the relationship is closed or restructured.
- **Controls:** All deceased-estate payouts above a threshold dual-approved; tracking dashboard for unresolved estates. **[Control Point]**
- **Evidence:** Succession documents; legal sufficiency note; payment records. **[Audit Evidence]**
- **Reference:** Estates and Court Orders Manual. **[Jurisdiction-Dependent]**

---

**SOP-039 — Lost / Damaged Certificate Replacement Under Indemnity**
- **Purpose:** Issue a duplicate certificate without exposing the Bank to double payment.
- **Trigger:** Customer reports a lost or damaged physical certificate.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Branch Manager.
- **Inputs:** Customer declaration; indemnity in approved form; notice period observation.
- **Procedure:**
  1. Officer records the loss against the original certificate series; the original is flagged "STOP".
  2. Customer executes the Bank's indemnity, witnessed as required.
  3. After the notice period, a duplicate is issued, marked "DUPLICATE" and cross-referenced to the original.
- **Controls:** Quarterly review of duplicate issuances; series register reconciled monthly. **[Control Point]**
- **Evidence:** Indemnity; series register entry; duplicate certificate copy. **[Audit Evidence]**
- **Reference:** Stationery Control Policy.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 8 — Dormancy, Unclaimed Balances & Escheatment

## 8.1 Dormancy Definition and Triggering Events

For the purposes of conventional time deposits, dormancy is the state into which an account passes when, after maturity, the depositor has not given an effective instruction (either to renew or to redeem) and cannot be reached through the customer's contact channels of record. Dormancy is distinct from the operational state of "matured-unclaimed", which is a transitional state pending tracing and reactivation.

## 8.2 Dormancy Timeline

The dormancy classification follows the timeline below, expressed against the maturity date (M) of the unclaimed deposit. **[Jurisdiction-Dependent]** numbers are illustrative and shall be replaced by the local statutory or supervisory timetable.

| State | Effective From | Operational Effect |
|---|---|---|
| Matured-Unclaimed | M + 0 | Proceeds parked in matured-unclaimed GL; no interest unless product specifies; customer contacted at M+1, M+30, M+90 |
| Inoperative | M + 90 | Inbound credits restricted; statements suppressed; tracing intensified |
| Dormant | M + 365 | Account flagged dormant; reactivation requires KYC refresh and customer authentication |
| Unclaimed (pre-escheatment) | M + 5 years | Final notification; listed for statutory transfer |
| Escheated | M + statutory period | Funds transferred to the regulator's unclaimed property fund; the Bank's liability is extinguished or transferred per local law |

## 8.3 Customer Tracing, Notification, and Reactivation

The Bank shall use reasonable means — registered post to the address of record, telephone contact, email, and, where consented, electronic messaging — to trace the depositor. The contact log shall be retained as evidence of reasonable effort. Customer-initiated reactivation requires identification verification, a KYC refresh appropriate to the period elapsed, and, where applicable, beneficial-ownership re-confirmation.

## 8.4 Escheatment / Transfer to Regulator or Unclaimed Property Fund

Annual escheatment is the statutory process by which long-unclaimed funds are remitted to the relevant authority. The escheatment listing shall be reviewed and signed off by the Operations Controller, the Compliance Officer, and the Board Audit Committee (or its delegate) prior to remittance. Once remitted, the Bank retains the case file to enable customer claim handling under SOP-043.

## 8.5 Reactivation After Escheatment

A customer who appears after escheatment may make a claim against the unclaimed property fund. The Bank's role is to verify identity, validate the claim against its records, certify the amount remitted, and facilitate the claimant's interaction with the authority. The Bank shall not pay the customer from its own resources for an escheated deposit.

### Standard Operating Practices in this Chapter

---

**SOP-040 — Dormancy Classification and Customer Notification (T+90 / T+180 / T+365)**
- **Purpose:** Move accounts through the dormancy timeline with appropriate notification.
- **Trigger:** Calendar advance for matured-unclaimed deposits.
- **Roles:** Maker — Operations Officer; Checker — Compliance Officer; Approver — Operations Controller.
- **Inputs:** Matured-unclaimed list; customer contact data; calendar.
- **Procedure:**
  1. CBS advances classification on schedule.
  2. Notifications are dispatched at T+1, T+30, T+90, T+180, and annually thereafter.
  3. Successful contacts re-open the case for reactivation (SOP-041).
  4. Each non-delivery is recorded; failed channels trigger alternative-channel attempts.
- **Controls:** Monthly dormancy ageing report; sampling of contact attempts. **[Control Point]**
- **Evidence:** Contact log; classification trail. **[Audit Evidence]**
- **Reference:** Dormancy Policy.

---

**SOP-041 — Customer Tracing and Reactivation Upon Contact**
- **Purpose:** Restore an active customer relationship and discharge the obligation.
- **Trigger:** Customer responds or presents at branch.
- **Roles:** Maker — Branch Officer; Checker — Branch Service Manager; Approver — Compliance for periods exceeding the refresh window.
- **Inputs:** Customer identification; updated KYC.
- **Procedure:**
  1. Officer authenticates the customer and conducts a fresh KYC.
  2. Operations reverses the dormancy flag in CBS.
  3. The matured proceeds are paid out per the customer's current instruction.
  4. The case is closed; the contact log is updated.
- **Controls:** Senior approval for reactivation after extended dormancy; **[Red Flag]** monitoring for reactivation by parties other than the original depositor. **[Control Point]**
- **Evidence:** KYC refresh; reactivation approval; payout record. **[Audit Evidence]**
- **Reference:** Dormancy Policy.

---

**SOP-042 — Annual Escheatment Listing, Board Attestation, and Statutory Remittance**
- **Purpose:** Discharge the Bank's statutory unclaimed-property obligation.
- **Trigger:** Annual escheatment calendar.
- **Roles:** Maker — Operations Officer; Checker — Compliance and Finance Officers; Approver — Board Audit Committee delegate.
- **Inputs:** Aged dormant list; statutory format file; remittance instrument.
- **Procedure:**
  1. Operations prepares the candidate list at the cut-off date.
  2. Compliance verifies that the tracing standard was met for each entry.
  3. Finance prepares the remittance instrument; the GL transfers the funds to escheatment payable; on settlement, the bank's liability is extinguished or transferred per local law.
  4. The board delegate signs off; the regulator-format file is submitted.
- **Controls:** Pre-remittance reconciliation between the candidate list and the GL movement; sign-off file retained. **[Control Point]**
- **Evidence:** Candidate list; reconciliation; board sign-off; submission acknowledgement. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Unclaimed Property statute.

---

**SOP-043 — Post-Escheatment Claim Handling**
- **Purpose:** Assist a customer who appears after escheatment without paying from the Bank's resources.
- **Trigger:** Customer claim received post-escheatment.
- **Roles:** Maker — Operations Officer; Checker — Compliance Officer; Approver — Head of Operations.
- **Inputs:** Customer claim; ID; case file from archive.
- **Procedure:**
  1. Officer retrieves the archived case file.
  2. Officer verifies identity and validates the claim.
  3. Officer issues a certificate of remittance to the claimant and directs them to the regulator/fund.
  4. The claim status is logged.
- **Controls:** Reconciliation between claims certified and any subsequent regulator confirmations received. **[Control Point]**
- **Evidence:** Claim file; certificate of remittance. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Unclaimed Property statute.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 9 — Accounting, Reconciliation, Regulatory & Tax Reporting

## 9.1 Chart of Accounts for the TD Book

The conventional time deposit book is supported by a structured chart of accounts that separates principal, accrual, interest expense, and tax liability balances by currency and product. At a minimum, the following GL families are maintained:

| GL Family | Code Family (Illustrative) | Description |
|---|---|---|
| TD Principal — Customer | 2210-* | Liability to depositors at par, by product and currency |
| TD Interest Payable | 2215-* | Accrued and unpaid interest |
| WHT Payable | 2270-* | Withholding tax deducted, pending statutory remittance |
| Matured-Unclaimed | 2280-* | Funds matured but not paid out / not reclaimed |
| Escheatment Payable | 2290-* | Funds awaiting remittance to unclaimed-property fund |
| Interest Expense — TD | 8110-* | Daily accrual P&L hit |
| Interest Expense Recovered (Break) | 8120-* | Recoveries via break cost |
| Fee Income — TD | 7110-* | Certificate replacement, statement fees, etc. |

Sub-ledger account discipline is the foundation of the reconciliations below.

## 9.2 Daily Subledger-to-GL Reconciliation

A daily reconciliation between the TD subledger (deposit-by-deposit) and the GL totals shall be performed. Differences shall be itemised, aged, and cleared. The reconciliation is signed off by Finance; a copy is held for audit. Period-end (month, quarter, year) reconciliations are subject to additional review by the Head of Finance and the external auditors during the engagement.

## 9.3 Liquidity & Basel Reporting

The time deposit book is a critical input into the Bank's liquidity and funding ratios under the Basel framework. The book provides stable funding under the Net Stable Funding Ratio (NSFR) and contributes to the cash outflows under the Liquidity Coverage Ratio (LCR), each with run-off factors differentiated by customer type (retail vs wholesale), insurance coverage (insured vs uninsured), and residual maturity.

The reporting data feed shall be reconciled to the subledger before submission. **[Jurisdiction-Dependent]** Run-off factors and segmentation reflect the local supervisory implementation of Basel.

## 9.4 Deposit Insurance: Coverage Limits, Premium, and SCV File

Where deposit insurance applies, the Bank shall maintain a Single Customer View (SCV) file containing per-depositor consolidated balances across the Bank's products, in a format prescribed by the insurance scheme. The SCV file shall be capable of being produced on demand within the scheme's required service-level (often 24–72 hours). The Bank shall pay the levy/premium to the scheme by the prescribed deadline.

**[Jurisdiction-Dependent]** Coverage limits per depositor per institution, eligibility of foreign currency, and treatment of joint accounts vary by scheme.

## 9.5 Tax Reporting

Three primary reporting obligations arise from the time deposit book:

- **Withholding tax** — periodic returns to the tax authority of WHT deducted at source, supported by the schedule of interest events.
- **Information returns** on interest paid (analogous to the U.S. Form 1099-INT) — annual statements of interest paid per recipient, where required.
- **FATCA and CRS** annual reporting of reportable accounts to the local tax authority for onward exchange with partner jurisdictions.

## 9.6 Statements, Confirmations, and Audit Confirmations to External Auditors

The Bank shall issue customer statements at the frequency prescribed by product or law (typically annually for TDs with no movement between booking and maturity). External-audit confirmation requests received in respect of depositors of the Bank shall be discharged via the central audit confirmation desk under SOP-048.

## 9.7 Management Information: TD Book MIS Pack

The Operating Committee receives a monthly TD book MIS pack covering: book size by tenor, currency, and product; weighted-average rate; net new money; rollover rate; break rate; cost of funds vs benchmark; concentration to top depositors; complaints volume and themes; control breaches and remediation status. The MIS pack is reconciled to the GL prior to circulation.

### Standard Operating Practices in this Chapter

---

**SOP-044 — Daily TD Subledger-to-GL Reconciliation and Break Investigation**
- **Purpose:** Maintain ledger integrity across the TD book.
- **Trigger:** End-of-day batch completion.
- **Roles:** Maker — Reconciler; Checker — Finance Manager; Approver — Head of Finance Operations.
- **Inputs:** Subledger extract; GL extract.
- **Procedure:**
  1. Reconciler matches subledger totals to GL totals by product and currency.
  2. Differences are itemised and assigned for investigation.
  3. The break inventory is aged; items older than two (2) business days are escalated.
  4. The reconciliation is signed off and archived.
- **Controls:** Independent of accrual maker; daily ageing dashboard. **[Control Point]**
- **Evidence:** Reconciliation file; sign-off. **[Audit Evidence]**
- **Reference:** Reconciliation Policy.

---

**SOP-045 — Monthly Deposit Insurance SCV File Preparation**
- **Purpose:** Maintain a production-ready Single Customer View for deposit insurance.
- **Trigger:** Monthly cycle; ad hoc on scheme request.
- **Roles:** Maker — SCV Production Officer; Checker — Finance Manager; Approver — Head of Finance Operations.
- **Inputs:** Customer master; deposit subledger; SCV format specification.
- **Procedure:**
  1. SCV Officer runs the SCV generation job.
  2. Reconciles total balance in the SCV to the GL.
  3. Validates structural correctness against the scheme schema.
  4. Stores the file with controls; tests retrieval within scheme SLA quarterly.
- **Controls:** Quarterly retrieval test; reconciliation to GL each cycle. **[Control Point]**
- **Evidence:** SCV file; reconciliation; retrieval test log. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Deposit Insurance Scheme rules.

---

**SOP-046 — Regulatory Liquidity Return (LCR/NSFR) Data Submission for the Deposit Book**
- **Purpose:** Provide accurate TD-book input into liquidity returns.
- **Trigger:** Reporting cycle (daily/monthly/quarterly per regulator).
- **Roles:** Maker — Regulatory Reporting Analyst; Checker — Treasury Risk; Approver — Head of Regulatory Reporting.
- **Inputs:** Subledger by customer type, residual maturity, insurance status; run-off factor table.
- **Procedure:**
  1. Analyst extracts and tags the TD book with regulatory dimensions.
  2. Treasury Risk reviews the segmentation and run-off application.
  3. The submission is reconciled to the subledger and to the GL.
  4. Submission is made via the regulator's portal; acknowledgement is filed.
- **Controls:** Pre-submission reconciliation; post-submission variance analysis vs prior period. **[Control Point]**
- **Evidence:** Submission file; reconciliation; acknowledgement. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Local Basel implementation.

---

**SOP-047 — Withholding Tax Return Filing and Remittance**
- **Purpose:** Discharge the Bank's withholding agent obligations on time and in full.
- **Trigger:** Statutory WHT cycle.
- **Roles:** Maker — Tax Operations Analyst; Checker — Finance Controller; Approver — Head of Tax.
- **Inputs:** WHT-event log; treaty / exemption certificates; return template.
- **Procedure:**
  1. Tax Operations reconciles the WHT GL to the WHT-event log.
  2. The return is prepared; treaty / exemption cases are individually supported.
  3. The remittance is settled to the tax authority by the statutory deadline.
  4. The acknowledgement is filed and the GL cleared.
- **Controls:** Annual reconciliation to annual interest payments; sample audit of treaty cases. **[Control Point]**
- **Evidence:** Return; remittance receipt; reconciliation. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Tax law.

---

**SOP-048 — External Audit Confirmation Response Handling**
- **Purpose:** Provide accurate balance and terms confirmations to external auditors under engagement.
- **Trigger:** Receipt of audit confirmation request.
- **Roles:** Maker — Audit Confirmation Desk Officer; Checker — Finance Manager; Approver — Head of Finance Operations.
- **Inputs:** Auditor request; customer authority where required; subledger.
- **Procedure:**
  1. Officer authenticates the auditor and the request.
  2. Officer reconciles the requested balances and terms to the subledger.
  3. The response is signed off and dispatched via the secure channel.
  4. The response copy is retained.
- **Controls:** Dual-control on dispatch; turn-around SLA monitoring. **[Control Point]**
- **Evidence:** Confirmation response; subledger extract; dispatch log. **[Audit Evidence]**
- **Reference:** External Audit Liaison Standard.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Chapter 10 — Controls, Audit, Fraud, Complaints & Business Continuity

## 10.1 Control Inventory and Testing Frequency

The control environment surrounding the TD book is captured in a Control Inventory, owned by the first line and tested at frequencies calibrated to risk. Each control bears a unique identifier (e.g., TD-CTRL-101), an owner, a tester, a testing frequency, and a tolerance. The Inventory is the bedrock against which the RCSA (Risk and Control Self-Assessment) is run quarterly.

**Control Testing Frequency (Illustrative)**

| Control ID | Description | Owner | Frequency | Tester |
|---|---|---|---|---|
| TD-CTRL-101 | Maker-checker on every booking | Branch | Each event | 1LoD self-check + 2LoD monthly sample |
| TD-CTRL-102 | Daily subledger-to-GL reconciliation | Finance Ops | Daily | 2LoD monthly sample |
| TD-CTRL-103 | KFS issuance and customer signature | Branch | Each event | 2LoD monthly sample |
| TD-CTRL-104 | KYC refresh by tier | Compliance | Monthly cycle | 2LoD quarterly |
| TD-CTRL-105 | Sanctions screening hit clearance | Compliance | Each event | 2LoD quarterly QA |
| TD-CTRL-106 | Rate sheet sign-off and CBS reconciliation | Treasury | Each rate change | 2LoD monthly |
| TD-CTRL-107 | WHT remittance and reconciliation | Tax Ops | Each cycle | 2LoD per cycle |
| TD-CTRL-108 | Dormancy classification | Operations | Monthly | 2LoD quarterly |
| TD-CTRL-109 | Escheatment listing sign-off | Operations | Annual | 3LoD on each escheatment |
| TD-CTRL-110 | Stationery series reconciliation | Branch | Monthly | 2LoD quarterly |

## 10.2 Segregation of Duties Matrix

No single person may perform conflicting roles in the booking, amendment, closure, and reconciliation of a deposit. The matrix below sets out the required separations.

| Activity | Initiate | Verify | Approve | Reconcile |
|---|---|---|---|---|
| Account opening | Officer | Service Manager | Branch Manager (above threshold) | Finance Ops |
| Rate exception | Relationship Manager | Branch Manager | Treasury / Head of Liabilities | Treasury Risk |
| Amendment of standing instruction | Officer | Service Manager | (callback if material) | — |
| Early withdrawal | Officer | Service Manager | Branch Manager / Ops Ctrl | Finance Ops |
| Hardship waiver | Branch / RM | Compliance | Head of Liabilities | Finance Ops |
| Escheatment | Operations | Compliance + Finance | Board delegate | Internal Audit (3LoD) |

## 10.3 Fraud Typologies and Red Flags Specific to Time Deposits

The Officer shall be alert to: ghost depositors (deposits booked without an underlying customer); suppressed or fictitious certificate series; amendments shortly before redemption that redirect proceeds to a new account; unusual proliferation of joint holders; sudden waiver of break cost in circumstances that benefit a specific party; rapid in-and-out activity inconsistent with the time-deposit purpose; collusion patterns between Officer and customer signalled by repeat business steered to a single Officer.

Where any of these **[Red Flag]** patterns are observed, the Officer shall escalate to the Branch Manager and Financial Crime under the Whistleblowing and Fraud Reporting Standard, and shall not discuss the case with the customer.

## 10.4 Internal Audit Cycle and Issue Remediation

Internal Audit covers the TD book on a risk-based cycle, typically not less than once every two years for material branches and once every three years across the network, with topical reviews in between. Audit issues are tracked to closure in the issue management system; "high" rated issues bear remediation deadlines not exceeding ninety (90) days; overdue items are reported to the Board Audit Committee.

## 10.5 Customer Complaints Handling

Complaints concerning time deposits — for example, rate disputes, break-cost disputes, certificate issues, dormancy disputes — are received through any of the Bank's complaint channels and are recorded centrally. Complaints are acknowledged within one (1) business day, investigated within fifteen (15) business days (extendable with customer consent), and resolved with a written response. Regulator-routed complaints follow the additional procedure described in SOP-050.

## 10.6 Business Continuity, Disaster Recovery, and Manual Workarounds

The TD book is identified as a critical business service. The Bank maintains a Business Continuity Plan with recovery time objectives (RTO) and recovery point objectives (RPO) calibrated for the TD book. Manual workarounds are documented for the core processes — booking, accrual, payment, redemption — so that the Bank can continue to honour its customer obligations during system unavailability. Quarterly BCP exercises include at least one TD-book scenario.

## 10.7 Training, Attestations, and Competency

All staff in roles named in section 1.5 shall complete role-based training on this manual upon joining, on every material amendment, and at least annually. Completion is recorded by Human Resources; non-completion bars the staff member from acting in that role.

### Standard Operating Practices in this Chapter

---

**SOP-049 — Quarterly Control Self-Assessment (RCSA) for the TD Book**
- **Purpose:** Provide first-line attestation on the design and operating effectiveness of TD-book controls.
- **Trigger:** Quarterly cycle.
- **Roles:** Maker — Control Owner per Inventory; Checker — Operational Risk Partner; Approver — Head of Liabilities.
- **Inputs:** Control Inventory; testing evidence; incident log; complaint themes.
- **Procedure:**
  1. Each control owner self-assesses against the Inventory, supported by testing evidence.
  2. The Operational Risk Partner challenges and aggregates.
  3. The aggregated RCSA is presented to the Head of Liabilities for sign-off.
  4. Material weaknesses are issued and tracked to closure.
- **Controls:** Aggregated RCSA reviewed by Operating Risk Committee; trend tracked. **[Control Point]**
- **Evidence:** Self-assessment; aggregated RCSA; sign-off. **[Audit Evidence]**
- **Reference:** Operational Risk Framework.

---

**SOP-050 — Customer Complaint Intake, Root-Cause Analysis, and Regulatory Escalation**
- **Purpose:** Resolve complaints, learn from them, and meet regulatory complaints reporting obligations.
- **Trigger:** Receipt of a complaint via any channel.
- **Roles:** Maker — Complaints Officer; Checker — Quality Assurance Officer; Approver — Head of Customer Experience.
- **Inputs:** Complaint detail; product and account record; communication history.
- **Procedure:**
  1. Officer acknowledges the complaint within one (1) business day.
  2. Officer investigates, drawing on Operations, Finance, and Compliance as required.
  3. Root-cause is identified; remediation actions are taken at customer level and, where systemic, at product/process level.
  4. A written response is issued within fifteen (15) business days, or an extension is sought with customer consent.
  5. Regulator-routed complaints follow the regulator's prescribed timeline and format; the regulator's case manager is the primary correspondent.
- **Controls:** Monthly complaints trend reporting; complaints feed into product review and RCSA. **[Control Point]**
- **Evidence:** Complaint file; written response; remediation actions; regulator correspondence. **[Audit Evidence]**
- **Reference:** **[Jurisdiction-Dependent]** Consumer Protection regulation; Complaints Handling Policy.

---

> *Local Compliance and Legal shall confirm all jurisdictional parameters before this chapter is operationalised.*

---

# Appendix A — Glossary

- **ACT/360, ACT/365, 30/360, ACT/ACT** — day-count conventions, see section 5.1.
- **ALCO** — Asset and Liability Committee; sets pricing and funding mandates.
- **ALM** — Asset and Liability Management.
- **Beneficial Owner (UBO)** — the natural person who ultimately owns or controls a customer.
- **Break Cost** — financial penalty applied on early withdrawal; see Chapter 7.
- **CDD** — Customer Due Diligence; the baseline KYC review.
- **CD / TD / FD** — Certificate of Deposit / Time Deposit / Fixed Deposit; equivalent terms.
- **CRS** — Common Reporting Standard (OECD) on automatic exchange of tax information.
- **CTR** — Cash Transaction Report; required disclosure above a threshold.
- **Day-Count Basis** — the denominator (e.g., 360, 365, actual) used in interest computation.
- **Deceased Estate Flag** — CBS marker restricting transactions on a deposit upon notice of demise.
- **Dormant Account** — an account meeting the dormancy criteria of section 8.1.
- **EDD** — Enhanced Due Diligence; deeper review for higher-risk relationships.
- **Escheatment** — statutory remittance of long-unclaimed funds to a regulator or public fund.
- **FATCA** — U.S. Foreign Account Tax Compliance Act and its local transposition.
- **GL** — General Ledger.
- **Indemnity** — formal undertaking to hold the Bank harmless against loss arising from a duplicate certificate or similar.
- **KFS** — Key Facts Statement; the consumer disclosure summary.
- **LCR** — Liquidity Coverage Ratio (Basel III).
- **Maker-Checker** — separation between transaction initiator and verifier.
- **Maturity Date** — the contractual date on which the deposit is repayable.
- **MLRO** — Money Laundering Reporting Officer.
- **NIM** — Net Interest Margin.
- **NSFR** — Net Stable Funding Ratio (Basel III).
- **PEP** — Politically Exposed Person.
- **PPD** — Product Programme Document; the governance file for a product.
- **PGC** — Product Governance Committee.
- **Principal** — the sum placed on deposit.
- **RCSA** — Risk and Control Self-Assessment.
- **Rollover** — automatic or instructed renewal of a deposit at maturity.
- **SCV** — Single Customer View; the deposit-insurance consolidation file.
- **SoF / SoW** — Source of Funds / Source of Wealth.
- **Standing Instruction** — a pre-recorded customer choice executed automatically by CBS.
- **Tenor** — the contractual life of the deposit.
- **Tiered Rate** — rate that varies by principal band or by customer segment.
- **Treasury Operations** — the back-office settlement of treasury transactions.
- **WHT** — Withholding Tax on interest paid to depositors.

---

# Appendix B — Acronym List

ALCO, ALM, AML, BCP, CBS, CDD, CRS, CTR, EDD, FATCA, FCY, FX, GL, KFS, KYC, LCR, MIS, MLRO, NIM, NSFR, PEP, PGC, PoA, PPD, QA, RACI, RCSA, RM, RTO/RPO, SCV, SDD, SLA, SoF, SoW, TD, UBO, WHT.

---

# Appendix C — Jurisdictional Parameters Workbook

Local Compliance and Legal shall populate this workbook before the manual is operationalised in any jurisdiction. The following placeholders identify all jurisdiction-dependent variables referenced in the chapters above. Each entry shall be confirmed in writing and dated.

| Ref | Item | Source | Value (to be populated) |
|---|---|---|---|
| J-01 | CTR (cash transaction reporting) threshold | AML statute / regulator | |
| J-02 | Currency-of-record statutory reporting thresholds | AML statute / regulator | |
| J-03 | Sanctions regimes applicable | Regulator / international lists | |
| J-04 | PEP definition and scope | AML statute | |
| J-05 | UBO disclosure threshold | AML statute / company law | |
| J-06 | FATCA local implementation | Tax authority | |
| J-07 | CRS local implementation and reporting deadline | Tax authority | |
| J-08 | WHT rate on interest — residents | Tax law | |
| J-09 | WHT rate on interest — non-residents | Tax law | |
| J-10 | Tax treaty entitlement procedure | Tax law / treaty network | |
| J-11 | Deposit insurance coverage limit per depositor per institution | Deposit insurance scheme | |
| J-12 | Deposit insurance eligibility — currency / customer type | Deposit insurance scheme | |
| J-13 | SCV file specification and SLA | Deposit insurance scheme | |
| J-14 | LCR run-off factors — retail / wholesale / uninsured | Regulator (Basel transposition) | |
| J-15 | NSFR available stable funding factors | Regulator (Basel transposition) | |
| J-16 | Cooling-off period for retail deposits | Consumer protection rule | |
| J-17 | Dormancy timeline — inoperative / dormant / unclaimed thresholds | Statute / regulator | |
| J-18 | Escheatment statutory period and remittance procedure | Unclaimed property statute | |
| J-19 | Estate / succession documentation accepted | Probate law | |
| J-20 | Cheque clearing days by instrument | Clearing house | |
| J-21 | Public holiday calendar — domestic and FCY | Calendar authority | |
| J-22 | Consumer complaints regulator and timeline | Consumer protection regulator | |
| J-23 | Record-retention period for closed deposits | Statute / regulator | |
| J-24 | Permitted maximum tenor for retail TDs | Regulator (where applicable) | |
| J-25 | Exchange-control eligibility for FCY deposits | Exchange control regulator | |

---

# Appendix D — Sample Journal Entries (Consolidated)

The following entries summarise the postings used across the manual. Account codes are illustrative.

> **Funding at Inception**
> ```
> Dr  1010-CASH-BRANCH                    USD 100,000.00
>    Cr  2210-TD-PRINCIPAL-CUST                USD 100,000.00
> ```
>
> **Daily Accrual**
> ```
> Dr  8110-INT-EXP-TD                     USD     11.64
>    Cr  2215-TD-INT-PAYABLE                    USD     11.64
> ```
>
> **Periodic Interest Payment (with WHT)**
> ```
> Dr  2215-TD-INT-PAYABLE                 USD  1,062.50
>    Cr  1110-CASA-CUST                         USD    902.13
>    Cr  2270-WHT-PAYABLE                       USD    159.38
> ```
>
> **Capitalisation at Sub-Period**
> ```
> Dr  2215-TD-INT-PAYABLE                 USD  1,062.50
>    Cr  2210-TD-PRINCIPAL-CUST                USD  1,062.50
> ```
>
> **Maturity Redemption**
> ```
> Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
> Dr  2215-TD-INT-PAYABLE                 USD  4,250.00
>    Cr  1110-CASA-CUST                         USD 104,250.00
> ```
>
> **Premature Closure with Break Cost**
> ```
> Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
> Dr  2215-TD-INT-PAYABLE                 USD  2,328.77
>    Cr  1110-CASA-CUST                         USD 101,164.38
>    Cr  8120-INT-EXP-RECOVERED                  USD  1,164.39
> ```
>
> **Transfer to Matured-Unclaimed (T = M)**
> ```
> Dr  2210-TD-PRINCIPAL-CUST              USD 100,000.00
> Dr  2215-TD-INT-PAYABLE                 USD  4,250.00
>    Cr  2280-MATURED-UNCLAIMED                 USD 104,250.00
> ```
>
> **Escheatment Remittance (Statutory)**
> ```
> Dr  2280-MATURED-UNCLAIMED              USD 104,250.00
>    Cr  2290-ESCHEATMENT-PAYABLE                USD 104,250.00
> Dr  2290-ESCHEATMENT-PAYABLE            USD 104,250.00
>    Cr  1010-CASH-CLEARING                      USD 104,250.00
> ```
>
> **Back-Value Adjustment Reversal (Illustrative)**
> ```
> Dr  2215-TD-INT-PAYABLE                 USD     50.00
>    Cr  8110-INT-EXP-TD                          USD     50.00
> Narrative: Back-value reversal of over-accrual identified on TD #...
> ```

---

# Appendix E — SOP Index

| SOP | Title | Chapter |
|---|---|---|
| SOP-001 | New product approval and PPD issuance | 1 |
| SOP-002 | Annual product review and product-line attestation | 1 |
| SOP-003 | Policy waiver request, approval, and logging | 1 |
| SOP-004 | Manual maintenance, versioning, and staff acknowledgement | 1 |
| SOP-005 | Daily/weekly rate sheet preparation and ALCO sign-off | 2 |
| SOP-006 | Promotional/campaign rate approval and expiry control | 2 |
| SOP-007 | KFS issuance and customer acknowledgement | 2 |
| SOP-008 | FCY TD eligibility check and FX confirmation | 2 |
| SOP-009 | Rate-exception (preferential pricing) approval and logging | 2 |
| SOP-010 | Individual customer onboarding and ID verification | 3 |
| SOP-011 | Corporate / trust / partnership onboarding and mandate capture | 3 |
| SOP-012 | Joint, minor, and PoA account onboarding | 3 |
| SOP-013 | PEP and sanctions screening, hit clearance, and L2/L3 escalation | 3 |
| SOP-014 | Enhanced Due Diligence (EDD) for high-risk customers | 3 |
| SOP-015 | FATCA/CRS self-certification capture and validation | 3 |
| SOP-016 | Periodic KYC refresh by risk tier | 3 |
| SOP-017 | Customer exit and de-risking decision | 3 |
| SOP-018 | Application intake, completeness check, and maker-checker booking | 4 |
| SOP-019 | Funding verification by channel and cleared-funds rule | 4 |
| SOP-020 | Cash deposit handling for TD funding (CTR thresholds) | 4 |
| SOP-021 | TD certificate / e-advice generation, dispatch, and acknowledgement | 4 |
| SOP-022 | Capture of maturity instruction and nominee details | 4 |
| SOP-023 | Same-day cancellation / cooling-off handling | 4 |
| SOP-024 | End-of-day interest accrual run and exception review | 5 |
| SOP-025 | Periodic interest payment to customer account and GL posting | 5 |
| SOP-026 | Withholding tax computation, deduction, and tax-GL sweep | 5 |
| SOP-027 | Back-value adjustment and interest recomputation | 5 |
| SOP-028 | Accrual reconciliation: subledger vs general ledger | 5 |
| SOP-029 | Holiday/weekend rollforward and value-date correction | 5 |
| SOP-030 | Pre-maturity notification (T-7 / T-3) and instruction confirmation | 6 |
| SOP-031 | Automatic rollover processing and rate-on-renewal application | 6 |
| SOP-032 | Amendment of standing maturity instruction | 6 |
| SOP-033 | Partial withdrawal processing where product permits | 6 |
| SOP-034 | Customer-initiated early withdrawal: intake and authority check | 7 |
| SOP-035 | Break-cost computation, approval, and customer disclosure | 7 |
| SOP-036 | Hardship/compassionate waiver approval and logging | 7 |
| SOP-037 | Maturity payout processing and customer settlement | 7 |
| SOP-038 | Deceased estate claim handling and disbursement | 7 |
| SOP-039 | Lost / damaged certificate replacement under indemnity | 7 |
| SOP-040 | Dormancy classification and customer notification | 8 |
| SOP-041 | Customer tracing and reactivation upon contact | 8 |
| SOP-042 | Annual escheatment listing, board attestation, and statutory remittance | 8 |
| SOP-043 | Post-escheatment claim handling | 8 |
| SOP-044 | Daily TD subledger-to-GL reconciliation and break investigation | 9 |
| SOP-045 | Monthly deposit insurance SCV file preparation | 9 |
| SOP-046 | Regulatory liquidity return (LCR/NSFR) data submission | 9 |
| SOP-047 | Withholding tax return filing and remittance | 9 |
| SOP-048 | External audit confirmation response handling | 9 |
| SOP-049 | Quarterly control self-assessment (RCSA) for the TD book | 10 |
| SOP-050 | Customer complaint intake, root-cause analysis, and regulatory escalation | 10 |

---

# Appendix F — Document Control & Version History

| Version | Date | Author / Owner | Approver | Summary of Change |
|---|---|---|---|---|
| 1.0 | (Effective date upon issuance) | Head of Retail & Wholesale Liabilities | Product Governance Committee | Initial issuance of the consolidated Conventional Time Deposit Banking Manual: 10 chapters, 50 SOPs, appendices A–F. |

**End of Manual.**

*This manual is the property of the Bank. Unauthorised disclosure is prohibited. The controlled electronic version published on the Bank's intranet is the sole authoritative copy.*
