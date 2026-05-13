# Lifewise KPI Dashboard Concept

This repository contains the working materials for the Lifewise Community Services KPI dashboard concept.

It is mainly for project teammates to review the current dashboard idea before it becomes a real Power BI dashboard.

## What To Open First

Open this file:

```text
powerbi_dashboard_concept/lifewise_powerbi_mockup.html
```

This is an interactive HTML mockup. It opens in a normal web browser such as Chrome, Edge, or Safari.

You do not need Power BI, coding software, or any special app to view it.

## How To Use The HTML Mockup

1. Download or open the repository folder.
2. Go to `powerbi_dashboard_concept`.
3. Double-click `lifewise_powerbi_mockup.html`.
4. Use the left-hand navigation to move between pages.
5. Use the service dropdown to switch between services.

If the page opens as code instead of a dashboard, right-click the file and choose **Open With** then select your web browser.

## What The Mockup Shows

The mockup has four pages.

### 1. Portfolio KPI Performance

This is the main dashboard view for Ann-Marie.

It shows:

- Portfolio-level KPI status cards.
- A Service × KPI performance matrix.
- RAG status: Red, Amber, Green, and Grey.
- Top alerts that need attention.

Important: this page is a concept demonstration. Some values are real, some are illustrative, and some are grey because evidence is still pending.

### 2. Service Detail

This page shows one selected service in more detail.

It includes:

- Service profile information.
- Funder / contract information.
- Source systems and evidence.
- KPI table.
- KPI performance snapshot.
- Follow-up questions.

For ARL, ECE, and Merge Café, the page includes example KPI cards and simple trend lines.

For Whānau Services, the page shows historical evaluation findings only. These are not current monthly performance results.

For low-readiness or scope-confirmation services, the page shows a placeholder explaining what still needs to be confirmed.

### 3. Service Manager Input

This page shows how service managers might enter monthly KPI numbers in the future.

It is not a live form. It is a mockup of a possible monthly input process.

It includes:

- A service selector.
- Monthly submission ribbon.
- Data source status.
- KPI input cards.
- Commentary boxes.
- Example trend chart.
- Save draft / submit buttons.

For ARL, ECE, and Merge Café, the page shows example input layouts.

For Whānau Services, Housing First, Youth Housing, Sustaining Tenancies, Addiction counselling, and Social enterprise, the page explains what still needs to be confirmed before an input form can be designed.

### 4. Project & Data Readiness

This page is for the project team.

It shows:

- Current-state readiness distribution.
- Service cards.
- Evidence completeness.
- Readiness matrix.
- Open follow-up actions.

This page should not be read as service performance. It is about whether the project has enough evidence and data structure to build a reliable dashboard.

## How To Read The Labels

The dashboard uses three types of data labels.

### Real

`Real` means the value comes from a client-provided or publicly referenced source.

Example:

- ARL CHRA 2025/26 Annual Monitoring Template.
- ECE Quality Plan 2026.
- Merge Café Service Manager response.
- Mana Whānau Final Evaluation 2020.

### [Illustrative]

`[Illustrative]` means the value is only a placeholder used to demonstrate dashboard logic.

It is not confirmed Lifewise performance data.

Illustrative values are included so reviewers can understand how the dashboard would look once real monthly values are supplied.

### Grey

Grey means the dashboard should not calculate performance yet.

Grey is used when one or more of these are missing:

- KPI definition.
- Target.
- Source field.
- Monthly actual value.
- Confirmed service scope.

Grey is not a performance failure. It means more evidence is needed.

## Important Interpretation Notes

- Page 1 is designed as an operational KPI dashboard concept, not just a readiness tracker.
- Page 4 keeps the readiness and evidence-gap work separate from performance monitoring.
- ARL / Community-Social Housing and ECE currently have the strongest evidence for early prototyping.
- Merge Café has clear targets, but KPI definitions and source mapping still need confirmation.
- Housing First, Youth Housing, Sustaining Tenancies, and Whānau Services remain discovery areas.
- Property team is a data owner / supporting source, not a service sector.
- Addiction counselling and Social enterprise are scope-confirmation items only.
- Whānau 89% / 94% figures are historical evaluation outcomes, not current monthly KPI performance.

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

The Excel workbook is the source of truth for the current-state assessment.

It separates:

- Client-provided facts.
- Current observations.
- Data readiness assessment.
- Follow-up questions.
- Dashboard design recommendations.

## Sample Data Files

The CSV files in `sample_data` are a future Power BI data model example.

They are not confirmed monthly performance data.

They show how a future dashboard could organise:

- Services.
- KPIs.
- Monthly KPI entries.
- Readiness status.
- Follow-up actions.

## Suggested Review Questions

When reviewing the HTML mockup, please consider:

1. Does Page 1 help Ann-Marie see service performance quickly?
2. Are Real, `[Illustrative]`, and Grey statuses clear enough?
3. Does Page 3 feel simple enough for service managers to use monthly?
4. Are any service rows missing or incorrectly grouped?
5. Which KPI definitions, targets, or source systems still need client confirmation?

## Recommended Next Steps

1. Share the HTML mockup with the project team for feedback.
2. Confirm dashboard scope with Ann-Marie.
3. Confirm KPI definitions and RAG targets for ARL, ECE, and Merge Café.
4. Obtain real monthly input files or exports.
5. Decide which services should be included in the first Power BI prototype.
