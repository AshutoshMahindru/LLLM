# Design Principles

## Version

| Field | Value |
|---|---|
| Version | 0.1 |
| Status | Draft |
| Date | 2026-06-29 |

## Principles

### 1. No Compromise

Critical infrastructure components must be high quality, reliable, supportable, and appropriate for long-term use.

### 2. No Overkill

Do not buy capability that has no realistic role in the architecture. Extra capability must be justified by redundancy, lifecycle, performance, or future expansion.

### 3. Amazon.in First

Physical procurement is Amazon.in-first. If unavailable, mark the item as not available on Amazon.in and document the alternative source.

### 4. Direct Product Links Only

Final procurement rows must use direct Amazon.in product pages and ASINs. Search links are unacceptable as final records.

### 5. One Source of Truth

Use one master procurement workbook and one GitHub repository. Avoid parallel uncontrolled lists.

### 6. Document the Why

Every major decision must be captured in an ADR or decision register entry.

### 7. Freeze Before Expanding

Complete and freeze one system before progressing to the next system.

### 8. Keep Systems Operable

Architecture must prioritize maintainability, recovery, monitoring, documentation, and practical operation over theoretical elegance.

### 9. Prefer Deterministic Validation

For document, Excel, and PowerPoint workflows, use deterministic tools and validators alongside AI models.

### 10. Security by Default

No exposed model services, no unmanaged secrets, no undocumented access paths, and no production dependency on memory-only configuration knowledge.
