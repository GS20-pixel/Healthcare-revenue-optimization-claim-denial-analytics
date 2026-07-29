# Entity Relationship Diagram (ERD)

The Power BI data model consists of nine healthcare tables connected through primary and foreign key relationships. The model links patient, provider, encounter, billing, and denial data to support healthcare revenue and claim denial analysis.

## Key Relationships

- Patients → Encounters
- Providers → Encounters
- Encounters → Claims & Billing
- Claims & Billing → Denials
- Encounters → Diagnoses
- Encounters → Procedures
- Encounters → Medications
- Encounters → Lab Tests