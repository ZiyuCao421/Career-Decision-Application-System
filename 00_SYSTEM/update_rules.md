# Update rules / 更新规则

1. Preserve raw source links and checked dates; append corrections rather than silently replacing material findings.
2. One application has one immutable `Application ID` and one record folder. One company entity has one immutable `Company ID`.
3. Add a row to an index when a record is created; update its `Last Updated` date whenever its substantive status changes.
4. Keep facts, unverified information, personal opinions, and rumours labelled separately.
5. Do not store national IDs, passwords, tokens, private recruiter contact details, full résumés, or other unnecessary personal data in the repository.
6. Use `N/A` only for an inapplicable assessment. Leave unknown data blank and record it as an unverified item where it affects a decision.
7. Do not overwrite the user's source résumé files. Store only non-sensitive references such as a resume version label.
8. Before commits, check IDs, date formats, controlled region/currency fields, CSV headers, and score weights.
9. Record the active application phase. In the `Broad Application` phase, do not reject a role solely because research or scoring is incomplete; document any explicit high-risk safety signal and the verification action instead.
