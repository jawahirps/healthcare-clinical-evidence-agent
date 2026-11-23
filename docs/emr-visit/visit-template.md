# EMR Visit Record — Template (DRAFT)

> Placeholders only. Tab names and fields are assumptions until checked against the live SLMC screens (`https://dxb6.simplexworld.com/SLMC/patientRegistration#tabEMR`). Fields marked `[unverified]` are from standard practice, not the live system. Do not enter real patient data in this file.

---

## Visit Header

| Field | Value |
|---|---|
| Visit ID | `[VISIT-ID]` |
| MRN | `[MRN]` |
| Encounter ID | `[ENCOUNTER-ID]` |
| Visit date/time | `[YYYY-MM-DD HH:MM]` |
| Visit type | `[new / follow-up / emergency / procedure / teleconsult / other]` |
| Facility / department | `[FACILITY]` / `[DEPARTMENT]` |
| Clinician | `[CLINICIAN-NAME]`, `[SPECIALTY]`, License `[LICENSE-NO]` `[unverified]` |
| Chief complaint | `[CHIEF-COMPLAINT]` |
| Status | `[registered / in-progress / completed / cancelled / no-show]` |

---

## Tab 1 — Registration

- Patient name: `[FULL-NAME]`
- Date of birth: `[DOB]`
- Sex: `[male / female / other / unknown]`
- Nationality: `[NATIONALITY]`
- Emirates ID: `[784-XXXX-XXXXXXX-X]` `[unverified]`
- Mobile: `[MOBILE]`
- Email: `[EMAIL]`
- Address: `[ADDRESS]`
- Emergency contact: `[NAME]`, `[RELATIONSHIP]`, `[PHONE]`
- Registration no.: `[REG-NO]`
- Consent signed: `[yes/no]`, date `[DATE]`
- ID verified: `[yes/no]`

## Tab 2 — Insurance `[unverified tab]`

- Payer: `[PAYER-NAME]` (ID `[PAYER-ID]`)
- Policy no.: `[POLICY-NO]`
- Member ID: `[MEMBER-ID]`
- Policy holder: `[HOLDER]`, relation `[RELATION]`
- Policy period: `[START]` to `[END]`
- Co-pay: `[PERCENT]`%
- Network tier: `[TIER]`

## Tab 3 — Vitals

| Measure | Value | Unit |
|---|---|---|
| Measured at | `[DATETIME]` | |
| Height | `[VALUE]` | cm |
| Weight | `[VALUE]` | kg |
| BMI | `[VALUE]` | kg/m² |
| Temperature | `[VALUE]` | °C |
| Pulse | `[VALUE]` | bpm |
| Respiratory rate | `[VALUE]` | /min |
| Blood pressure | `[SYS]` / `[DIA]` | mmHg |
| SpO₂ | `[VALUE]` | % |
| Pain score | `[0–10]` | |

## Tab 4 — History

- Present illness: `[HPI]`
- Past medical history: `[PMH]`
- Past surgical history: `[PSH]`
- Allergies: `[SUBSTANCE]` — reaction `[REACTION]` — severity `[mild/moderate/severe/unknown]`
- Family history: `[FHX]`
- Smoking: `[STATUS]`
- Alcohol: `[STATUS]`
- Occupation: `[OCCUPATION]`

## Tab 5 — Examination

- General appearance: `[FINDINGS]`
- Systems reviewed: `[SYSTEM]`: `[FINDING]` (repeat per system)

## Tab 6 — Diagnosis

| Type | ICD-10-CM `[unverified code system]` | Description | Onset |
|---|---|---|---|
| `[primary / secondary / provisional / rule-out]` | `[CODE]` | `[DESCRIPTION]` | `[DATE]` |

## Tab 7 — Orders

| Order ID | Type | Code | Description | Ordered at | Status |
|---|---|---|---|---|---|
| `[ID]` | `[lab / imaging / referral / other]` | `[CODE]` | `[DESC]` | `[DATETIME]` | `[STATUS]` |

## Tab 8 — Results

| Order ID | Test | Value | Unit | Reference range | Flag | Resulted at |
|---|---|---|---|---|---|---|
| `[ID]` | `[TEST]` | `[VALUE]` | `[UNIT]` | `[RANGE]` | `[normal/high/low/critical]` | `[DATETIME]` |

## Tab 9 — Medications

| Name | Generic | Dose | Route | Frequency | Duration | Qty | Action |
|---|---|---|---|---|---|---|---|
| `[NAME]` | `[GENERIC]` | `[DOSE]` | `[ROUTE]` | `[FREQ]` | `[DURATION]` | `[QTY]` | `[new/continue/change/stop]` |

## Tab 10 — Procedures

| Code (CPT) | Description | Performed at | Performed by | Notes |
|---|---|---|---|---|
| `[CODE]` | `[DESC]` | `[DATETIME]` | `[NAME]` | `[NOTES]` |

## Tab 11 — Plan

- Assessment: `[ASSESSMENT]`
- Plan: `[PLAN]`
- Follow-up: `[DATE]`
- Patient education: `[TEXT]`
- Referrals: `[REFERRAL]`

## Tab 12 — Billing

- Invoice no.: `[INVOICE-NO]`
- Line items: `[CODE]` · `[DESC]` · qty `[QTY]` · unit `[PRICE]` · total `[TOTAL]`
- Currency: `AED`
- Total: `[TOTAL]`
- Payment status: `[unpaid / partial / paid / waived]`

## Tab 13 — Attachments

- `[FILE-NAME]` · `[MIME-TYPE]` · uploaded `[DATETIME]`

## Tab 14 — Pre-authorization (eClaimLink) `[unverified]`

- Request no.: `[REQUEST-NO]`
- Status: `[draft / submitted / approved / rejected / pended]`
- Requested services: `[CODE]` · `[DESC]` · qty `[QTY]` · est. `[AMOUNT]`
- Approval no.: `[APPROVAL-NO]`
- Approved at: `[DATETIME]`
- Valid until: `[DATE]`
