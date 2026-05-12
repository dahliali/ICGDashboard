# Lifewise KPI Dashboard Concept - Power BI Page Specification

Source of truth: `service_level_master_current_state_v0.4_ece_quality_plan.xlsx`

Design principle: the dashboard must separate operational KPI performance from data readiness and evidence gaps. Missing targets, unconfirmed definitions, missing monthly feeds, or unconfirmed scope should use a grey status, not a red performance failure.

## Shared Model Assumptions

- Refresh cadence: monthly input, with near-real-time enough for portfolio oversight.
- Microsoft 365 fit: SharePoint / Teams-hosted Excel or list input tables can be used first; Power BI can later connect to governed source systems where available.
- RAG status only applies where a KPI target and KPI definition are confirmed.
- Readiness status is separate from performance status.
- Property team is a data owner / supporting source, not a service sector.
- Addiction counselling and Social enterprise are scope-confirmation items until service-specific evidence is received.

## Page 1: Portfolio Overview

### Purpose
Give Ann-Marie a one-page portfolio view of service coverage, data readiness, prototype candidates, low-readiness areas, and open follow-up workload.

### Target User
Ann-Marie Searchfield and senior portfolio stakeholders.

### Visuals Needed
- KPI cards:
  - Total rows / services in current-state table
  - Medium readiness count
  - Medium-Low readiness count
  - Low readiness count
  - Unknown / scope confirmation count
  - Open high-priority follow-ups
- Service readiness matrix:
  - Rows: Service sector / owner
  - Columns: Entity type, Data readiness, Evidence type, Reporting frequency, Service manager
  - Conditional formatting on Data readiness
- Prototype candidate panel:
  - ARL / Community-Social Housing
  - ECE
  - Merge Café as simple KPI demonstration pending definition confirmation
- Discovery / scope panel:
  - Housing First
  - Youth Housing
  - Sustaining Tenancies
  - Whānau Services
  - Addiction counselling
  - Social enterprise
- Donut or stacked bar:
  - Count of rows by Data readiness
- Follow-up priority bar:
  - Count of actions by Category and Priority

### Fields Used
- Service Dimension:
  - ServiceID
  - ServiceName
  - EntityType
  - ServiceManager
  - FunderContract
  - ReportingFrequency
  - IsServiceSector
  - DesignRole
- Data Readiness Table:
  - ServiceID
  - ReadinessLevel
  - EvidenceType
  - CurrentIssues
  - FollowUpNeeded
- Follow-up Actions Table:
  - Category
  - QuestionTask
  - SuggestedOwner
  - Priority
  - RelatedServiceID

### Filters / Slicers
- Data readiness
- Entity type
- Service sector / owner
- Suggested owner
- Follow-up priority

### RAG Logic
- This page primarily shows readiness status, not KPI performance.
- Readiness colour logic:
  - Medium: blue
  - Medium-Low: amber
  - Low: red / dark amber for readiness risk only
  - N/A: neutral grey
  - Unknown / Scope confirmation required: purple / grey
- KPI performance RAG should not be shown for services without confirmed targets and definitions.

### Notes / Caveats
- Red readiness does not mean poor service performance. It means insufficient evidence for dashboard-ready reporting.
- ARL and ECE have the strongest current evidence but still require monthly-feed and mapping confirmation.
- Property team should be shown as a supporting source, not counted as a service performance area.

## Page 2: Service Detail

### Purpose
Allow a service manager or portfolio lead to select one service and inspect its KPIs, source systems, target status, readiness, issues, and follow-up questions.

### Target User
Ann-Marie and service managers.

### Visuals Needed
- Service selector slicer.
- Service summary card:
  - Service sector / owner
  - Entity type
  - Service manager
  - Funder / contract
  - Reporting frequency
  - Data readiness
- KPI table:
  - KPI name
  - Target value
  - Target status
  - Latest month value
  - RAG status
  - Definition status
  - Source system
- Trend chart:
  - Monthly KPI value by month for selected KPI
  - Target line where confirmed
  - Grey placeholder state where target or definition is not confirmed
- Current issues / observations panel:
  - Client-provided observations only
- Evidence panel:
  - Evidence type
  - Data source
  - Systems
- Follow-up actions table:
  - Question / task
  - Why it matters
  - Suggested owner
  - Priority

### Fields Used
- Service Dimension:
  - ServiceID
  - ServiceName
  - EntityType
  - FunderContract
  - ReportingFrequency
  - ServiceManager
- KPI Dimension:
  - KPIID
  - ServiceID
  - KPIName
  - TargetValue
  - TargetStatus
  - DefinitionStatus
  - SourceSystem
  - ReportingStream
- Monthly KPI Fact:
  - Month
  - ServiceID
  - KPIID
  - ActualValue
  - TargetValue
  - RAGStatus
  - DataStatus
  - Comment
- Data Readiness Table:
  - ReadinessLevel
  - CurrentIssues
  - EvidenceType
  - FollowUpNeeded
- Follow-up Actions Table:
  - RelatedServiceID
  - Category
  - QuestionTask
  - Priority

### Filters / Slicers
- Service
- KPI
- Month
- Reporting stream
- RAG status
- Data status

### RAG Logic
- Green: actual meets or exceeds confirmed target, based on confirmed KPI direction.
- Amber: actual is near target but below threshold, only where KPI direction and tolerance are confirmed.
- Red: actual misses confirmed target, only where KPI direction, target, and definition are confirmed.
- Grey:
  - Target not confirmed
  - Definition not confirmed
  - Source field mapping not confirmed
  - Monthly feed not proven
  - Scope confirmation required
- For this concept, only Merge Café and selected ECE targets can demonstrate target-based status. ARL figures are formal annual data but need RAG target confirmation before performance RAG.

### Notes / Caveats
- Do not compare service performance across sectors until KPI definitions and reporting cadence are standardised.
- Follow-up actions should be visible on the service detail page so data gaps are not hidden behind visuals.
- Where a KPI is confirmed as tracked but no monthly value exists, show "No monthly feed confirmed" instead of blank.

## Page 3: Data Readiness & Follow-up

### Purpose
Make evidence gaps, data capture risks, definition issues, and scope-confirmation items visible and actionable.

### Target User
Project team, Ann-Marie, service managers, and data owners.

### Visuals Needed
- Readiness definition table:
  - High
  - Medium
  - Medium-Low
  - Low
  - N/A
  - Unknown / Scope confirmation required
- Readiness by service matrix:
  - Service sector / owner
  - Evidence type
  - Data readiness
  - Current issues
  - Follow-up still needed
- Follow-up action tracker:
  - Category
  - Question / task
  - Suggested owner
  - Priority
  - Status
  - Due date
- Scope confirmation panel:
  - Addiction counselling
  - Social enterprise
- Data capture risk panel:
  - Whānau Services
  - Housing First
  - Youth Housing
  - Sustaining Tenancies

### Fields Used
- Data Readiness Table:
  - ServiceID
  - ReadinessLevel
  - EvidenceType
  - CurrentIssues
  - FollowUpNeeded
  - ReadinessDefinition
- Follow-up Actions Table:
  - FollowUpID
  - RelatedServiceID
  - Category
  - QuestionTask
  - WhyItMatters
  - SuggestedOwner
  - Priority
  - Status
  - DueDate
- Service Dimension:
  - ServiceName
  - EntityType

### Filters / Slicers
- Readiness level
- Category
- Priority
- Suggested owner
- Follow-up status
- Entity type

### RAG Logic
- This page uses readiness colour coding, not KPI performance RAG.
- Grey is used for N/A and unconfirmed scope.
- Low readiness should be treated as evidence risk, not service underperformance.

### Notes / Caveats
- The purpose of this page is to drive follow-up and evidence closure before dashboard schema is locked.
- The page should include a clear note: "Readiness status is not a judgement of service performance."
- Addiction counselling and Social enterprise should not appear as performance services until scope is confirmed.

## Page 4: Monthly Input Concept

### Purpose
Show how service managers could enter or validate monthly KPI values in a Microsoft 365-compatible workflow before full automation is available.

### Target User
Service managers, data owners, project team.

### Visuals Needed
- Monthly input grid:
  - Month
  - Service
  - KPI
  - Actual value
  - Target value
  - Definition status
  - Source system
  - Data status
  - Submitter
  - Reviewer
  - Comments
- Input completeness cards:
  - Expected entries
  - Submitted entries
  - Missing entries
  - Entries blocked by unconfirmed target/definition
- Data quality warning table:
  - Grey rows for target not confirmed, definition not confirmed, or source field not mapped
- Simple trend preview:
  - Selected KPI actual values by month
  - Target line where confirmed

### Fields Used
- Monthly KPI Fact:
  - Month
  - ServiceID
  - KPIID
  - ActualValue
  - TargetValue
  - RAGStatus
  - DataStatus
  - Submitter
  - Reviewer
  - Comment
- KPI Dimension:
  - KPIName
  - TargetStatus
  - DefinitionStatus
  - SourceSystem
- Service Dimension:
  - ServiceName
  - ServiceManager
- Data Readiness Table:
  - ReadinessLevel

### Filters / Slicers
- Month
- Service
- Service manager
- KPI
- Data status
- RAG status

### RAG Logic
- RAG is only calculated when:
  - KPI definition is confirmed
  - Target is confirmed
  - Actual value is available
  - Direction of good performance is known
- Grey status examples:
  - Target not confirmed
  - Definition not confirmed
  - Monthly feed not proven
  - Scope confirmation required
  - N/A supporting source

### Notes / Caveats
- Early implementation can use SharePoint Lists or controlled Excel tables stored in Teams / SharePoint.
- Power BI should consume the input table rather than act as the writeback tool unless a Power Apps writeback layer is later introduced.
- The input workflow should include review and sign-off fields to avoid unclear ownership of final numbers.
- Monthly input should not force services with Low or Unknown readiness into artificial KPI reporting before discovery is complete.

