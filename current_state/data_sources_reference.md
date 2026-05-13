# Lifewise Dashboard — Data Sources Reference

## Purpose

This document lists every data point used in the Lifewise KPI Dashboard mockup, its source, and its classification (real vs. illustrative). Use this for:

1. Report appendix — to cite data sources in the ICG deliverable
2. Client conversation — to be transparent about what is real vs. placeholder
3. Future updates — to track which placeholders need replacement once real data is supplied

---

## Source Classification

| Category | Description | Visual treatment in dashboard |
|---|---|---|
| **Real (client-provided)** | Sourced from documents/emails supplied by Lifewise | Source label + tooltip |
| **Real (Lifewise public)** | Sourced from Lifewise's publicly available reports | Source label + tooltip |
| **Real (NZ public register)** | Sourced from NZ Charities Register or official records | Source label + tooltip |
| **Illustrative** | Placeholder values generated to demonstrate dashboard concept | `[Illustrative]` tag, italic grey |
| **Grey / Pending** | No data available; evidence pending | Grey RAG indicator + status text |

---

## Source 1: ARL CHRA 2025/26 Annual Monitoring Template

**Document**: `CHRAKeyPerformanceMeasureReportingTemplate202526AnnualMonitoring__ARL.xlsx`

**Provided by**: Michael Chapman (Property team), via Maraea Mokaraka

**Date received**: 5 May 2026

**Status**: Internal Lifewise / Airedale Residential Limited (ARL) document. Project team has access via email attachment.

**Citation in report**:
> "ARL CHRA 2025/26 Annual Monitoring Template, supplied by Lifewise Property team (Michael Chapman) via email, 5 May 2026."

### Data points used:

| KPM | Measure | Value | Used in dashboard |
|---|---|---|---|
| KPM 2 | Total tenancy exits | 107 | Page 1 matrix; Page 3 input form |
| KPM 2 | Tenancy terminations | 37 (of which 25 RTA breaches) | Page 3 input form |
| KPM 4 | Tenancy exits (occupancy calculation) | 94 | Page 3 input form note |
| KPM 6 | Non-urgent repairs completed within 14 days | 169 / 241 = 70% | Page 1 alert; Page 3 input form |
| KPM 6 | Urgent repairs | 0 (not separately maintained) | Page 3 input form note |

### Notes:
- The three tenancy-exit-related figures (KPM2 exits 107, KPM2 terminations 37, KPM4 exits 94) need definition clarification with reporting owner before dashboard mapping is finalised.
- ARL workbook is formal annual evidence, not a proven monthly dashboard feed.

---

## Source 2: Lifewise ECE Quality Plan 2026

**Document**: `Quality_Plan-Service_Specific-ECE_Lifewise_Services_2026.docx`

**Provided by**: Maraea Mokaraka (forwarding ECE Service Manager response)

**Date received**: 5 May 2026

**Status**: Internal Lifewise quality plan document for Waimumu Road Preschool and Royal Road Preschool.

**Citation in report**:
> "Lifewise ECE Quality Plan 2026 (Waimumu Road & Royal Road Preschool), supplied by Lifewise via email, 5 May 2026."

### Data points used (all targets, no actuals):

| KPI | Target | Used in dashboard |
|---|---|---|
| Occupancy / utilisation | ~90% | Page 1 ECE row; Page 2 KPI snapshot |
| Funded child hours by category | Meet/exceed budget | Page 2 KPI snapshot |
| Staff qualification mix | ~80% qualified | Page 2 KPI snapshot |
| Mandatory training compliance | ≥95% | Page 1 ECE row; Page 2 KPI snapshot |
| Incident reporting within 24h | 100% | Page 1 ECE row; Page 2 KPI snapshot |
| Complaints acknowledged within policy timeframe | 100% | Page 2 KPI snapshot |
| Internal audit completion | 100% | Page 1 ECE row; Page 2 KPI snapshot |
| CAPA closed on time | ≥90% | Page 2 KPI snapshot |
| Regulatory self-audit | 100% | Page 2 KPI snapshot |
| Priority whānau engagement | 80–100% | Page 1 ECE row; Page 2 KPI snapshot |

### Notes:
- Targets only — no actual monthly performance values provided.
- Document is a quality plan / scoping response, not a raw monthly KPI dataset.

---

## Source 3: Merge Café Service Manager Response

**Email**: Paula Bold Wilson (Service Manager Merge), via Maraea Mokaraka

**Date received**: 5 May 2026

**Status**: Service Manager email response to project team data request.

**Citation in report**:
> "Merge Café Service Manager response (Paula Bold Wilson), supplied via Lifewise email, 5 May 2026."

### Data points used (targets only):

| KPI | Target | Used in dashboard |
|---|---|---|
| Immediate needs met | 85% | Page 1 Merge row; Page 2; Page 3 |
| Continued engagement | 85% | Page 1 Merge row; Page 2; Page 3 |
| Connected to community services | 50% | Page 1 Merge row; Page 2; Page 3 |

### Additional context (not used as data points but informs dashboard design):
- Same KPI set reported to MHUD monthly and Auckland Council annually
- Data sources: Recordbase (primary), Excel, Microsoft Forms (H&S), Lightspeed (café operations)
- Excel KPI sheet is linked to funding release and shared with finance business partner

### Notes:
- KPI numerator / denominator definitions not yet confirmed.
- Recordbase field mapping not yet confirmed.
- Actual performance values not provided.

---

## Source 4: Mana Whānau Final Evaluation 2020

**Document**: `Mana-whanau-evaluation.pdf` (Point & Associates, September 2020)

**Public URL**: https://communityresearch.org.nz/wp-content/uploads/formidable/8/Mana-whanau-evaluation.pdf

**Authors**: Alex Woodley, Point & Associates Limited (commissioned by Lifewise / Wesley Community Action)

**Publication date**: September 2020 (covers period 2018 - July 2020)

**Status**: Publicly available evaluation report published on Community Research NZ.

**Citation in report**:
> "Woodley, A. (2020). *Mana Whānau Final Evaluation*. Point & Associates, commissioned by Lifewise. Published on Community Research NZ. Available at: communityresearch.org.nz"

### Data points used:

| Indicator | Value | Used in dashboard |
|---|---|---|
| Total whānau participated (2-year period) | 44 (Auckland: 26; Porirua: 18) | Page 2 Whānau Services historical panel |
| Total tamariki | 139 | Page 2 Whānau Services historical panel |
| **Whānau retained tamariki** | 39 / 44 = **89%** | Page 1 small "Historical reference" badge (NOT a KPI cell); Page 2 historical panel |
| **Tamariki living safely with whānau** | 130 / 139 = **94%** | Page 1 small "Historical reference" badge (NOT a KPI cell); Page 2 historical panel |
| Māori representation | 48% | Page 2 historical panel |
| Pasifika representation | 27% | Page 2 historical panel |
| NZ European representation | 37% | Page 2 historical panel |
| Programme duration | 6 months | Page 2 context |

**Restrictions on Page 1 usage of 89% / 94%**:

These figures may appear on Page 1 only as a small "Historical outcome reference" badge or tooltip. They must NOT:
- Appear as a current KPI RAG cell
- Affect the Overall RAG for the Whānau row (which remains Grey)
- Contribute to Section 1 portfolio health metrics (KPIs meeting target / Red count / Amber count)
- Be visually styled the same as current performance values

### Notes:
- Historical 2018-2020 data only. Current monthly data not available.
- A newer Mana Whānau Evaluation Report (March 2026) is referenced on the Lifewise public website (https://www.lifewise.org.nz/). Public webpage indicates key findings (e.g., 87% parents retained/regained care; 94% whānau still safely caring 1–7 years later), but the full report has not been provided to the project team. **Treat as public webpage finding only, not as a confirmed dashboard data source**. Listed in follow-up data requests.

---

## Source 5: Lifewise Trust Public Information

**Sources**:
- Lifewise About page: https://www.lifewise.org.nz/about-lifewise/
- NZ Charities Register: https://register.charities.govt.nz/Charity/CC40248
- Lifewise NZ LinkedIn: https://nz.linkedin.com/company/lifewisenz

**Status**: Publicly available organisational information.

**Citation in report**:
> "Lifewise Trust organisational information sourced from Lifewise public website and New Zealand Charities Register (CC40248)."

### Data points used (context only):

| Indicator | Value | Used in dashboard |
|---|---|---|
| Charity registration | CC40248 | Footer / About panel |
| Balance date | June 30 | Context |
| Staff count | 320 | Context |
| Trusts | 3 (Lifewise, APT, MMN) | Context |
| Services | 10 | Context |
| Sites | 11 | Context |
| Operating regions | Northland, Auckland, Waikato, Bay of Plenty | Context |

---

## Source 6: Lifewise Housing Services ICG Fact Sheet

**Document**: `Lifewise Housing Services_ ICG fact sheet .docx`

**Provided by**: Maraea Mokaraka (Community Housing Manager)

**Date received**: 5 May 2026

**Status**: Background fact sheet / questionnaire-style response.

**Citation in report**:
> "Lifewise Housing Services background fact sheet, supplied by Maraea Mokaraka (Community Housing Manager), 5 May 2026."

### Data points used (categorical only, not performance metrics):

| Service | Used in dashboard |
|---|---|
| Housing First — described as 1 SM per sector, KPI categories listed (no targets) | Page 1 row 4; Page 4 readiness |
| Youth Housing — described as 1 SM per sector, KPI categories listed (no targets) | Page 1 row 5; Page 4 readiness |
| Sustaining Tenancies — described as 1 SM per sector, KPI categories listed (no targets) | Page 1 row 6; Page 4 readiness |

### Notes:
- Document uses hedging language ("typically", "usually") indicating responses are general descriptions, not confirmed reporting structure.
- No targets, no field definitions, no monthly data, no named service managers.
- Readiness classified as **Low** in master current-state assessment.

---

## Source 7: Whānau Services Email Response

**Email**: Sher Gestro, via Maraea Mokaraka

**Date received**: 7 May 2026

**Status**: Service team response describing current state and future desired data capture.

**Citation in report**:
> "Whānau Services current-state response (Sher Gestro), supplied via Lifewise email, 7 May 2026."

### Data points used (categorical only):

| Indicator | Used in dashboard |
|---|---|
| Contracts: OT (Mana Whānau), MSD (Whānau Resilience), MoJ (Parenting through Separation) | Page 1 Whānau row contract column |
| KPI categories listed: families receiving intervention, FTE, declined referrals, waitlist, completion, etc. | Page 2 Service Detail KPI list (no targets) |
| Data source: Recordbase + manual capture | Page 2 systems |

### Notes:
- Response explicitly states "There are substantial gaps of recording of information."
- Future desired data fields (whānau history, trauma, mental health, etc.) are wishlist items, not confirmed current KPIs.

---

## Source 8: Property Team Response

**Email**: Michael Chapman, via Maraea Mokaraka (with CHRA template attachment)

**Date received**: 5 May 2026

**Status**: Internal team email response.

**Citation in report**:
> "Lifewise Property team response (Michael Chapman), supplied via Lifewise email, 5 May 2026."

### Data points used:

| Information | Used in dashboard |
|---|---|
| Property team is data owner, not service sector | Page 4 readiness; Service Detail entity type |
| Community / Social Housing includes Housing First and Youth Housing | Page 4 context note |
| Data sources: PMS, finance systems, Excel trackers | Page 1 footer; Service Detail |
| Review monthly, sometimes weekly | Service Detail frequency |

---

## Source 9: ICG Project Brief

**Document**: `Client_Project_Brief_Lifewise.pdf`

**Provided by**: ICG / Lifewise

**Date received**: Project initiation

**Status**: Formal client brief defining project deliverables.

**Citation in report**:
> "ICG Project Brief for Lifewise engagement, Semester 1 2026."

### Data points used:

| Information | Used in dashboard |
|---|---|
| Lifewise service areas mention "addiction counselling" and "social enterprise" | Page 1 Rows 8-9 as **scope placeholders only** (not confirmed service rows); Page 4 scope confirmation |
| Example metrics: bed nights, counsellor contact volumes, staffing levels | Reference for KPI types only — NOT linked to specific services |
| Stakeholder: Ann-Marie Searchfield (GM Community Services) | Dashboard primary user |

**Restrictions on Rows 8-9 (Addiction / Social Enterprise)**:

- Treat as scope placeholders, NOT confirmed dashboard rows
- All KPI cells must remain Grey
- Must NOT be counted in any portfolio aggregate (total services, KPIs meeting target, etc.)
- Visually distinct (e.g., muted styling, lower opacity) so client cannot misread them as "in scope but not yet performing"
- Project brief mentions these as Lifewise service areas, but no service-specific KPI evidence has been received. The brief does not constitute scope confirmation.

---

## Illustrative Data Inventory

The following data points are **NOT from any real source** — they are placeholder values generated by the project team to demonstrate dashboard logic. All are clearly marked `[Illustrative]` in the dashboard.

### Important note on ARL targets

The ARL CHRA 2025/26 Annual Monitoring Template contains *measures* (KPM 1–7 with specific sub-measures) and *figures*, but does NOT explicitly state internal RAG thresholds or targets for most KPMs. Any "target" used for ARL in the dashboard (e.g., rent arrears <3%, repairs ≥90%, turnaround <25 days) is an **illustrative threshold invented by the project team for demonstration purposes only**. These thresholds:

- Are labelled `[Illustrative threshold]` in the dashboard
- Should NOT be cited as Lifewise's actual performance targets
- Require confirmation from ARL reporting owner before any real use

### ARL illustrative actuals AND illustrative thresholds

| KPI | Illustrative actual | Illustrative threshold | Why illustrative |
|---|---|---|---|
| KPM 1 Rent arrears | $91,261 (4.9%) | <3% (NOT in CHRA) | Neither actual nor target provided |
| KPM 3 Turnaround time | 22 days | <25 days (NOT in CHRA) | Neither actual nor target provided |
| KPM 4 Occupancy rate | 90.5% | ~90% (NOT in CHRA) | Neither actual nor target provided |
| KPM 5 Complaints | 12 cases, median 8 days | TBC | Neither actual nor target provided |
| KPM 6 Non-urgent repairs (target only — actual 70% is REAL) | actual is real (169/241) | ≥90% (NOT in CHRA) | Target % not specified; only 14-day timeframe comes from CHRA |
| KPM 7 Tenant satisfaction | 76% | TBC | Neither actual nor target provided |
| ARL 12-month trend (any KPI) | rising/falling pattern | — | No historical actuals provided |

### ECE illustrative actuals

| KPI | Illustrative value | Why illustrative |
|---|---|---|
| Occupancy | 91% | No monthly actual provided |
| Training compliance | 96% | No monthly actual provided |
| Incident timeliness 24h | 92% | No monthly actual provided |
| Audit completion | 100% | No monthly actual provided |
| Priority whānau engagement | 85% | No monthly actual provided |
| ECE 12-month trend | 89 → 91 (stable) | No historical actuals provided |

### Merge Café illustrative actuals

| KPI | Illustrative value | Why illustrative |
|---|---|---|
| Immediate needs met | 87% | Target known (85%), actual not provided |
| Continued engagement | 86% | Target known (85%), actual not provided |
| Community connections | 38% | Target known (50%), actual not provided |
| Merge 12-month trend | 51 → 38 (declining) | No historical actuals provided |

### Portfolio aggregate illustrative

| Metric | Value in dashboard | Notes |
|---|---|---|
| KPIs meeting target | 67% `[Illustrative]` | Based on illustrative current actuals for ARL/ECE/Merge Café only |
| Red — action needed | 2 `[Illustrative]` | Counts illustrative red cells across ARL/ECE/Merge Café only |
| Amber — at risk | 3 `[Illustrative]` | Counts illustrative amber cells across ARL/ECE/Merge Café only |
| Trend "+4% vs last month" | `[Illustrative]` | Invented for demonstration |
| Submissions on time | **TBC (not 5/7)** | Client has not supplied monthly submission completion log. Tile should show "TBC" or remain greyed until real submission tracking data exists. Do NOT show a fake count like "5/7". |

**Important**: All portfolio aggregates exclude:
- Whānau Services historical 89%/94% (those are 2018-2020 outcomes, not current month)
- Housing First / Youth Housing / Sustaining Tenancies (Discovery — no KPI structure confirmed)
- Whānau Services current month (data capture gaps)
- Addiction Counselling and Social Enterprise (scope placeholders only)

---

## Suggested Report Appendix Wording

> ### Appendix A: Data Sources
>
> The dashboard mockup presented in this report uses a combination of real Lifewise data (sourced from client-provided documents and publicly available reports) and illustrative placeholder values (used to demonstrate dashboard logic).
>
> **Real data sources**:
> - ARL CHRA 2025/26 Annual Monitoring Template (client-supplied, 5 May 2026): tenancy exit figures (KPM2 = 107, terminations = 37; KPM4 = 94) and repair timeframes (169/241 = 70% within 14 days)
> - Lifewise ECE Quality Plan 2026 (client-supplied, 5 May 2026): all 10 ECE KPI targets
> - Merge Café Service Manager response (Paula Bold Wilson, client-supplied via Lifewise, 5 May 2026): 3 KPI targets (85% / 85% / 50%)
> - Mana Whānau Final Evaluation (Woodley, 2020, publicly available via Community Research NZ): historical outcome data for Whānau Services (89% whānau retention, 94% tamariki retention, n=44/139, 2018-2020)
> - Lifewise Trust organisational information (NZ Charities Register CC40248 and Lifewise public website)
>
> **Illustrative data**: All current monthly actual performance values, trend lines, portfolio aggregate metrics, and ARL RAG thresholds (except where explicitly noted as CHRA-derived) are illustrative placeholders generated by the project team. These are clearly marked `[Illustrative]` or `[Illustrative threshold]` in the dashboard interface. Real performance data and confirmed RAG thresholds are to be supplied by Lifewise before dashboard implementation.

> **Important note on ARL targets**: The CHRA template provides measures and figures but does not state explicit RAG thresholds. Any threshold shown for ARL KPIs (e.g., rent arrears <3%, repairs ≥90%, turnaround <25 days) is illustrative and requires confirmation from ARL reporting owner.

> **No data**: Housing First, Youth Housing, Sustaining Tenancies, Whānau Services (current monthly), Addiction Counselling, and Social Enterprise are shown with Grey indicators reflecting current evidence gaps. These services require further client engagement before dashboard design can be finalised.

---

## Recommended next data requests to client

To replace illustrative values with real data, request from Ann-Marie / Maraea:

1. **Merge Café**: One month of recent actual performance values for the 3 KPIs (e.g., October 2025 figures for immediate needs met, continued engagement, community connections)
2. **ECE**: One month of recent occupancy, training compliance, and incident timeliness values for both Waimumu Road and Royal Road
3. **ARL**: Any monthly snapshot of rent arrears, turnaround time, or tenant satisfaction (to supplement annual CHRA data)
4. **Whānau Services 2026 evaluation**: Full text of March 2026 Mana Whānau Evaluation Report (referenced on Lifewise website)
5. **Housing First / YH / ST**: Sample monthly report or KPI tracker showing actual KPI structure, targets, and any recent values
6. **Scope confirmation**: Written confirmation of whether Addiction Counselling and Social Enterprise are in dashboard scope; if yes, identify reporting owner and contract reference
