# CAMP workflow / 工作流

## Operating principle

CAMP is **human-led, AI-assisted**. The user verifies facts and makes all application and employment decisions. No document or automation may submit an application, send a recruiter message, or make an external commitment.

## Four stages

1. **Application intake** — create an `Application ID` in `02_APPLICATIONS/application_index.csv`, then copy the application template into `02_APPLICATIONS/records/YYYY/APP-####/`.
2. **Company & job investigation** — create or link a `Company ID`, record evidence in the company profile and the application's `investigation.md`. Important evidence requires source, URL, checked date, summary, confidence, and notes.
3. **Application review** — record Opportunity Score and Personal Fit Score independently. Ratings are 1–5 or `N/A`; do not infer missing values as zero. Record risk flags separately.
4. **Follow-up & analytics** — append interview events and outcomes. Update the application status and review weekly patterns without replacing source records.

## Standard lifecycle

`Saved` → `Applied` → `Screening` → `Assessment` → `Interview` → `Offer` / `Rejected` / `Withdrawn` / `Closed`

Use one current status in the index. Keep the detailed chronology in `feedback.md` and interview records.

## Identifiers

- `Application ID`: `APP-0001`, sequential and never reused.
- `Company ID`: `COMP-0001`, sequential and never reused.
- `Interview ID`: `INT-0001`, sequential and never reused.
- Dates: ISO 8601 (`YYYY-MM-DD`); datetimes use ISO 8601 with timezone.

## Region handling

Use `Country/Region` and `Currency` explicitly. Mainland China and Singapore evidence, registration details, work-authorisation notes, and employment-contract entities must remain distinct. Leave region-specific fields blank or `N/A` when inapplicable.
