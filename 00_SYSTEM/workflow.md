# CAMP workflow / 工作流

## Operating principle

CAMP is **human-led, AI-assisted**. The user verifies facts and makes all application and employment decisions. No document or automation may submit an application, send a recruiter message, or make an external commitment.

## Four stages

1. **Application intake** — create an `Application ID` in `02_APPLICATIONS/application_index.csv`, then copy the application template into `02_APPLICATIONS/records/YYYY/APP-####/`.
2. **Company & job investigation** — create or link a `Company ID`, record evidence in the company profile and the application's `investigation.md`. Important evidence requires source, URL, checked date, summary, confidence, and notes.
3. **Application review** — first record the current application phase, then record Opportunity Score and Personal Fit Score independently. Ratings are 1–5 or `N/A`; do not infer missing values as zero. Record the independent Job Safety Assessment and risk flags separately.
4. **Follow-up & analytics** — append interview events and outcomes. Update the application status and review weekly patterns without replacing source records.

## Standard lifecycle

`Saved` → `Applied` → `Screening` → `Assessment` → `Interview` → `Offer` / `Rejected` / `Withdrawn` / `Closed`

Use one current status in the index. Keep the detailed chronology in `feedback.md` and interview records.

## Dynamic application strategy

The evaluation system supports decisions; it does not replace them. During the **Broad Application / 海投** phase, the primary objective is efficient first-interview conversion. A partial Opportunity Score, incomplete company research, or less-than-perfect fit should not by itself remove a role from the candidate pool. Explicit high-risk safety signals warrant a pause or further verification.

Review the phase at least weekly and when interview feedback, available time, or graduation proximity materially changes. Possible phases: `Broad Application`, `Focused Application`, `Interview Conversion`, `Offer Decision`.

## Identifiers

- `Application ID`: `APP-0001`, sequential and never reused.
- `Company ID`: `COMP-0001`, sequential and never reused.
- `Interview ID`: `INT-0001`, sequential and never reused.
- Dates: ISO 8601 (`YYYY-MM-DD`); datetimes use ISO 8601 with timezone.

## Region handling

Use `Country/Region` and `Currency` explicitly. Mainland China and Singapore evidence, registration details, work-authorisation notes, and employment-contract entities must remain distinct. Leave region-specific fields blank or `N/A` when inapplicable.
