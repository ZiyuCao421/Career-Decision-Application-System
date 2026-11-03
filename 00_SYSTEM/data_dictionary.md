# Data dictionary / 数据字典

## Shared conventions

| Field | Rule |
|---|---|
| IDs | `APP-####`, `COMP-####`, `INT-####`; unique, immutable, and cross-referenced exactly. |
| Dates | ISO 8601 `YYYY-MM-DD`; missing values are blank. |
| Country/Region | Controlled values: `Mainland China`, `Singapore`, `Other`. |
| Currency | ISO 4217, e.g. `CNY`, `SGD`; never infer across regions. |
| Evidence classification | `Verified Fact`, `Unverified Information`, `Personal Opinion`, `Rumour`. |
| Confidence | `High`, `Medium`, `Low`, or blank. |

## Core indexes

| File | Primary key | Purpose |
|---|---|---|
| `02_APPLICATIONS/application_index.csv` | Application ID | One row per application or saved role. |
| `03_COMPANIES/company_index.csv` | Company ID | One row per legal/hiring entity under investigation. |
| `04_MARKET/job_market.csv` | Market Record ID | Dated market observation, not a job application. |
| `05_INTERVIEWS/interview_index.csv` | Interview ID | One row per interview or assessment event. |

## Controlled statuses

Application Status: `Saved`, `Applied`, `Screening`, `Assessment`, `Interview`, `Offer`, `Rejected`, `Withdrawn`, `Closed`.

Application Phase: `Broad Application`, `Focused Application`, `Interview Conversion`, `Offer Decision`.

Risk Level: `Low Risk`, `Needs Observation`, `High Risk`, `Not Assessed`.

Job Safety Assessment Status: `Not Assessed`, `Needs Verification`, `Clear on checked items`, `High Concern`.

Scoring coverage is the sum of assessed weights divided by 100. A score may be blank when no dimension is assessed.
