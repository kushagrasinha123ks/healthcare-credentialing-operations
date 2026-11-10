# U.S. Healthcare Credentialing Operations

An independent portfolio project that follows a provider file from credential verification through payer enrollment and decision handoff. The main case models California physician licensure, National Provider Identifier (NPI) verification, continuing medical education (CME) evidence review, and individual Original Medicare Part B enrollment.

All case records, identifiers, evidence references, and decisions are synthetic. The workbooks use a fixed November 10, 2026 snapshot so the examples can be reproduced.

## Start here

1. Read the [end-to-end case study](pdf/case-study-end-to-end-credentialing-operations-workflow.pdf) for the workflow and decision points.
2. Open both workbooks and filter **Tracker** for `PRV-001`. Follow the missing course completion certificate on `VER-003` and the corresponding hold on `ENR-001`. The hold reflects a simulated client policy.
3. On a copy, change the as-of date in **Controls** to see how follow-up priorities change. Compare `ENR-002`, which has an overdue external response deadline, and `ENR-003`, which needs effective-date and scope confirmation.

## Excel workbooks

| Workbook | What it tracks |
| --- | --- |
| [Provider Credential Verification Tracker](workbooks/provider-credential-verification-tracker.xlsx) | License, NPI, and CME evidence checks, including source references, discrepancies, reviewer disposition, and license expiry |
| [Enrollment Application Processing Tracker](workbooks/enrollment-application-processing-tracker.xlsx) | Packet review, submission evidence, internal and external deadlines, payer decisions, and effective dates |

Each workbook includes 12 synthetic records, dropdown validation, calculated exceptions, and a dashboard with a ranked follow-up queue. The **Controls** tab explains timing settings and source references.

## Research and operating documents

| Deliverable | PDF | Word |
| --- | --- | --- |
| U.S. Healthcare Provider Credentialing Research Report | [Read](pdf/us-healthcare-provider-credentialing-research-report.pdf) | [Download](docx/us-healthcare-provider-credentialing-research-report.docx) |
| Provider License Verification SOP | [Read](pdf/provider-license-verification-sop.pdf) | [Download](docx/provider-license-verification-sop.docx) |
| Provider Enrollment Application Processing SOP | [Read](pdf/provider-enrollment-application-processing-sop.pdf) | [Download](docx/provider-enrollment-application-processing-sop.docx) |
| Data Validation and Discrepancy Resolution Guidelines | [Read](pdf/data-validation-and-discrepancy-resolution-guidelines.pdf) | [Download](docx/data-validation-and-discrepancy-resolution-guidelines.docx) |
| Provider and Client Email Communication Templates | [Read](pdf/provider-and-client-email-communication-templates.pdf) | [Download](docx/provider-and-client-email-communication-templates.docx) |
| End-to-End Credentialing Operations Case Study | [Read](pdf/case-study-end-to-end-credentialing-operations-workflow.pdf) | [Download](docx/case-study-end-to-end-credentialing-operations-workflow.docx) |

## Sources and validation

- The research report records findings, limitations, and access dates for 17 public primary sources, including CMS, the Medical Board of California, and the eCFR. It distinguishes program requirements from the portfolio's simulated operating controls.
- Both workbooks were recalculated in LibreOffice Calc. Tests covered duplicate IDs, missing evidence, overdue requests, approval scope and effective-date checks, and release after documented review.
- The Word documents and PDFs were reopened and checked for layout and matching source links.
