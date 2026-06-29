# AI Infrastructure Design Authority

## Version 0.1 — Architecture & Procurement Baseline

| Field | Value |
|---|---|
| Status | Draft Baseline |
| Version | 0.1 |
| Date | 2026-06-29 |
| Scope | Private AI infrastructure |
| Owner | Ashutosh Mahindru |

## 1. Purpose

This document establishes the architecture, procurement methodology, governance model, documentation standards, and roadmap for the private AI infrastructure project.

The repository and related procurement workbook are intended to become the single source of truth for the system.

## 2. Vision

Design and build a private AI laboratory capable of running large local AI workloads while remaining secure, maintainable, extensible, and fully documented.

The infrastructure shall support:

- local large language model inference;
- document generation;
- spreadsheet and financial model generation;
- PowerPoint and presentation generation;
- coding agents;
- research agents;
- RAG and knowledge management;
- secure remote access;
- reproducible operations.

## 3. Current Hardware Direction

| Layer | Current / Planned Hardware | Role |
|---|---|---|
| Mobile | Google Pixel 10 Pro Fold, 16 GB memory | Mobile terminal, scanner, voice capture, approval device |
| Workstation | Apple MacBook Pro M5 Max, 128 GB memory | Control plane, development workstation, artifact review |
| AI Compute | 2 × NVIDIA DGX Spark | Local AI execution cluster |

## 4. Infrastructure Layers

1. Compute
2. Network
3. Storage
4. Power
5. Rack and environment
6. Workspace
7. Mobile
8. Security
9. AI platform
10. Operations
11. Documentation

## 5. Governing Principles

- No compromise on quality.
- No overkill without measurable technical benefit.
- Amazon.in first for physical procurement.
- One master procurement workbook.
- Every major decision must be captured as an ADR.
- Every artifact must be version-controlled where practical.
- Every completed system must be frozen before moving to the next.
- Every component must have a traceable role in the system.

## 6. Required Project Artifacts

- Procurement database
- Asset register
- Warranty register
- Architecture Decision Records
- Decision register
- Assumptions register
- Risk register
- Knowledge register
- Configuration register
- Cable schedule
- Rack layout
- Network diagrams
- Operations manual
- Runbooks

## 7. Procurement Methodology

Each product class follows this workflow:

1. Enumerate viable Amazon.in candidates.
2. Compare specifications.
3. Eliminate unsuitable options.
4. Select the recommended SKU.
5. Record rejected alternatives.
6. Document rationale.
7. Update budget.
8. Freeze the decision.

No search URLs are acceptable as final procurement links. Final rows require direct Amazon.in product pages and ASINs, unless a component is explicitly marked unavailable on Amazon.in.

## 8. Repository Governance

The GitHub repository is the source-controlled engineering record. The master workbook remains the procurement database, while Markdown files capture architecture, decisions, risks, assumptions, runbooks, and operational standards.

## 9. Active Phase

Current active phase: Network System / Batch 2A.

The Network System will be completed to zero unresolved procurement rows before moving to Storage.
