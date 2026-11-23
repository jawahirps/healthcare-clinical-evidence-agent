# Pre-Authorization Request — Draft (NOT SUBMITTED)

Target: eClaimLink pre-authorization form (`https://apps.eclaimlink.ae/eAuth/PR.aspx`).

> I could not open this form. The fields below are a placeholder draft. Confirm every field label and required flag against the live form before use. Nothing here has been submitted to the payer.

## 1. Provider
- Facility name: `[FACILITY]`
- Facility licence no.: `[LICENCE]`
- Treating clinician: `[NAME]`, specialty `[SPECIALTY]`, licence `[LICENCE]`

## 2. Patient and member
- Patient name: `[NAME]`
- Emirates ID: `[784-XXXX-XXXXXXX-X]`
- Date of birth: `[DOB]`
- Sex: `[SEX]`
- Payer: `[PAYER]`
- Policy no.: `[POLICY]`
- Member ID: `[MEMBER-ID]`

## 3. Encounter
- Encounter / visit ID: `[ENCOUNTER-ID]`
- Expected admission or visit date: `[DATE]`
- Visit type: `[TYPE]`
- Chief complaint: `[COMPLAINT]`

## 4. Diagnosis
- Primary: `[ICD-10-CM CODE]` `[DESCRIPTION]`
- Secondary: `[CODE]` `[DESCRIPTION]`

## 5. Requested services
| Service code | Description | Qty | Est. amount (AED) | Justification |
|---|---|---|---|---|
| `[CODE]` | `[DESC]` | `[QTY]` | `[AMOUNT]` | `[CLINICAL REASON]` |

## 6. Clinical justification
`[NARRATIVE — link to supporting results and history from the visit record]`

## 7. Attachments
- `[DOCUMENT NAME]` — `[TYPE]`

## 8. Declaration
`[Signature block — to be completed by the authorised clinician. Not to be filled in by automation.]`
