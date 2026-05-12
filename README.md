# Lifewise KPI Dashboard Concept

This repository contains the current-state analysis and Power BI dashboard concept pack for the Lifewise Community Services KPI dashboard project.

## Purpose

The dashboard concept is designed to support:

- Centralised operational reporting across Lifewise Community Services.
- Ann-Marie's portfolio oversight.
- Monthly KPI input and trend analysis by service managers.
- RAG status against confirmed targets.
- Practical implementation in a Microsoft 365 environment.

The materials intentionally separate:

- Client-provided facts and current-state evidence.
- Data readiness and evidence gaps.
- Consultant dashboard design recommendations.
- Future sample data model structure.

## Repository Contents

```text
current_state/
  service_level_master_current_state_v0.4_ece_quality_plan.xlsx

powerbi_dashboard_concept/
  powerbi_page_specification.md
  lifewise_powerbi_mockup.html
  sample_data/
    service_dimension.csv
    kpi_dimension.csv
    monthly_kpi_fact.csv
    data_readiness_table.csv
    follow_up_actions_table.csv
```

## Current-State Workbook

The Excel workbook is the source of truth for the current-state assessment. It includes:

- Master Current State
- Summary
- Readiness Standard
- Follow-up Actions
- Email Evidence
- Dashboard Design Recommendation

The workbook distinguishes facts, observations, readiness assessment, and consultant recommendations.

## Power BI Concept Pack

The Power BI concept pack includes:

- A page-by-page dashboard specification.
- A browser-based HTML mockup that looks and behaves like a Power BI concept dashboard.
- CSV sample tables for a future Power BI data model.

The four proposed dashboard pages are:

1. Portfolio Overview
2. Service Detail
3. Data Readiness & Follow-up
4. Monthly Input Concept

## Sample Data Model

The sample CSV files are a data model skeleton, not confirmed monthly KPI performance data.

They are designed to show how a future Power BI implementation could structure:

- Service dimension data
- KPI dimension data
- Monthly KPI fact input
- Data readiness evidence
- Follow-up actions

Blank actual values and grey statuses are intentional. They indicate missing data, unconfirmed targets, unconfirmed KPI definitions, or unconfirmed source-field mapping.

## Design Rules

- ARL / Community-Social Housing and ECE are the strongest current prototype candidates.
- Merge Cafe can be used as a simple KPI demonstration case once KPI definitions are confirmed.
- Housing First, Youth Housing, Sustaining Tenancies, and Whanau Services require further discovery before dashboard schema is locked.
- Property team is treated as a data owner / supporting source, not a service sector.
- Addiction counselling and Social enterprise are scope-confirmation items until service-specific evidence is received.
- Grey status is used for missing data, unconfirmed targets, or unconfirmed definitions. These should not be marked as red performance failures.

## Implementation Notes

This concept is practical for a Microsoft 365 and Power BI implementation:

- Early monthly input can use SharePoint Lists or controlled Excel tables stored in Teams / SharePoint.
- Power BI should consume the input table rather than act as the writeback tool.
- A Power Apps writeback layer could be considered later if needed.
- Readiness status should not be interpreted as service performance.

## Recommended Next Steps

1. Confirm dashboard scope with Ann-Marie.
2. Confirm KPI definitions and RAG targets for prototype candidates.
3. Obtain actual monthly input templates or exports for ARL, ECE, and Merge Cafe.
4. Confirm whether low-readiness services have stable monthly data capture.
5. Decide whether the first Power BI prototype should focus on ARL, ECE, and Merge Cafe only.

