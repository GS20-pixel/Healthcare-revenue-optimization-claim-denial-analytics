# Data Dictionary

## Dataset Overview

The project uses the **CA Hospital Dataset (Q1 2025)** consisting of nine related tables. These tables represent different aspects of hospital operations, patient care, insurance claims, and billing.

---

## Tables

| Table Name | Description | Records |
|------------|-------------|--------:|
| Patients | Patient demographic information | 60,000 |
| Providers | Healthcare provider information | 1,491 |
| Encounters | Patient visit records | 70,000 |
| Diagnoses | Diagnosis details for each encounter | 70,000 |
| Procedures | Medical procedures performed | 126,021 |
| Medications | Prescribed medications | 94,498 |
| Lab Tests | Laboratory test records | 54,537 |
| Claims & Billing | Insurance claims and billing details | 70,000 |
| Denials | Claim denial information | 5,998 |

---

# Key Tables Used for Analysis

## Patients

**Purpose:** Stores patient demographic information.

| Column | Description |
|--------|-------------|
| patient_id | Unique patient identifier |
| gender | Patient gender |
| age | Patient age |
| state | Patient location |

---

## Providers

**Purpose:** Stores healthcare provider information.

| Column | Description |
|--------|-------------|
| provider_id | Unique provider identifier |
| provider_name | Healthcare provider name |
| department | Medical department |

---

## Encounters

**Purpose:** Stores patient visit details.

| Column | Description |
|--------|-------------|
| encounter_id | Unique encounter ID |
| patient_id | Linked patient |
| provider_id | Linked provider |
| encounter_date | Date of visit |

---

## Claims & Billing

**Purpose:** Stores insurance claim and payment information.

| Column | Description |
|--------|-------------|
| claim_id | Unique claim identifier |
| insurance_provider | Insurance company |
| claim_billing_date | Billing date |
| billed_amount | Total billed amount |
| paid_amount | Amount received |
| claim_status | Claim status |
| revenue_leakage | Difference between billed and paid amount |

---

## Denials

**Purpose:** Stores denied insurance claims.

| Column | Description |
|--------|-------------|
| claim_id | Related claim |
| denial_reason | Reason for denial |
| denied_amount | Amount denied |
| denial_date | Date of denial |
| appeal_status | Appeal outcome |

---

## Relationship Summary

The analysis combines patient, provider, encounter, billing, and denial data to evaluate

- Revenue performance
- Insurance provider performance
- Claim approval and denial trends
- Revenue leakage
- Operational insights