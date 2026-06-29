# LLLM Meta-Model Specification

## Version 0.1

| Field | Value |
|---|---|
| Status | Draft |
| Version | 0.1 |
| Date | 2026-06-29 |
| Scope | Enterprise architecture, procurement, infrastructure, AI platform, operations |

## 1. Purpose

The LLLM Meta-Model defines the canonical information structure for the entire programme.

The intent is to prevent uncontrolled duplication across Excel, Coda, Logseq, Markdown, diagrams, procurement files, configuration records, and operational manuals.

## 2. Core Principle

Model once. Generate many views.

A component, product, requirement, decision, asset, or configuration should be represented once in the canonical model. Documents, workbooks, diagrams, registers, and dashboards are projections of that model.

## 3. Top-Level Entity Families

| Family | Purpose |
|---|---|
| Governance | Project, requirement, decision, risk, issue, standard |
| Architecture | system, subsystem, capability, interface, dependency |
| Procurement | product, vendor, seller, price, quote, order |
| Physical Estate | asset, location, rack, port, cable, power outlet |
| Configuration | configuration item, setting, policy, credential reference |
| Validation | test, acceptance criterion, benchmark, evidence |
| Knowledge | document, datasheet, manual, firmware, support reference |
| Operations | runbook, procedure, maintenance event, incident, change |

## 4. Canonical Entity Types

- Project
- Requirement
- Architecture Decision
- System
- Subsystem
- Capability
- Component
- Product
- Vendor
- Seller
- Asset
- Configuration Item
- Configuration Profile
- Interface
- Port
- Cable
- Location
- Rack
- Power Circuit
- Document
- Knowledge Reference
- Risk
- Issue
- Test
- Procedure
- Change
- Maintenance Event

## 5. Relationship Philosophy

Relationships are explicit, typed, and directional.

Examples:

- Requirement is implemented by System.
- System contains Component.
- Component is fulfilled by Product.
- Product is procured from Seller.
- Product becomes Asset after purchase.
- Asset is installed in Location.
- Asset is configured by Configuration Profile.
- Configuration Profile is validated by Test.
- Component is documented by Knowledge Reference.

## 6. Universal Identification

Every durable object receives a stable ID. IDs must be human-readable, typed, and sequence-based.

Examples:

- REQ-NET-001
- SYS-NET-001
- CMP-SW-001
- PRD-NET-001
- AST-NET-001
- CFG-FW-001
- ADR-0001
- RISK-001
- TEST-NET-001

## 7. Lifecycle Model

All durable entities follow a controlled lifecycle:

1. Draft
2. Review
3. Approved
4. Implemented
5. Operational
6. Deprecated
7. Archived

Not every entity reaches every state, but every entity must have a lifecycle state.

## 8. View Generation

The following artifacts are model views:

| View | Source Entities |
|---|---|
| Procurement workbook | Component + Product + Vendor + Seller + Price |
| Asset register | Asset + Product + Location + Warranty |
| Warranty register | Asset + Vendor + Warranty |
| Decision register | Architecture Decision |
| Requirements matrix | Requirement + System + Test |
| Network diagram | System + Interface + Port + Cable |
| Rack layout | Asset + Rack + Location |
| Configuration register | Configuration Item + Configuration Profile |
| Knowledge register | Product + Knowledge Reference |

## 9. Governance Rules

- No final procurement row without a requirement or design rationale.
- No final product recommendation without alternatives considered.
- No deployed asset without asset ID.
- No configuration without version and owner.
- No accepted system without validation evidence.
- No change without change record once the baseline is frozen.

## 10. Current Implementation State

The meta-model is initially represented as Markdown catalogues in GitHub.

Later projections may be implemented in:

- Excel workbook
- Coda database
- Logseq graph
- SQLite/PostgreSQL
- YAML/JSON files
- generated Markdown documentation
