# World Bank Data Analysis and Visualization in Excel

## Project Overview

This project contains two completed Microsoft Excel exercises focused on turning development data into accessible, decision-oriented visualizations. Exercise 1 explores **primary school enrolment (% gross)** across income groups, world regions, and hypothetical categories using PivotTables, charts, and a consolidated dashboard. Exercise 2 explores **data storytelling and chart design**, including reorganizing data for comparison, examining enrolment trends, stacked bar distributions, and geographical representations.

## Files

| Workbook | Description |
| --- | --- |
| `1-Module 5 - Execise 1 - Dashboard (1) workdone.xlsx` | Exercise 1: enrolment analysis, PivotTables, Figures 4A–4C, and an Excel dashboard. |
| `Module 5 - Exercise 2 - Basic Visualizations done.xlsx` | Exercise 2: introductory chart redesign, data organization, income-group comparisons, stacked bars, and mapping-oriented worksheets. |

## Data Sources and Measures

- **Primary source:** World Bank, *World Development Indicators* (the source sheets indicate a last update of **24 February 2026**).
- **Indicator:** `SE.PRM.ENRR` — **School enrollment, primary (% gross)**.
- **Interpretation:** Gross enrolment is the total number of pupils enrolled in primary education, regardless of age, expressed as a percentage of the population of official primary-school age. Values **can exceed 100%**.
- **Geographic metadata:** Country/economy-to-region and income-group labels held in the workbooks.
- **Hypothetical Metric A/B/C:** An analysis/demo grouping in Exercise 1, **not an official World Bank indicator**.

## Workbook 1 — Exercise 1: Dashboard

### Main worksheets

| Sheet | Purpose |
| --- | --- |
| `Raw Data` | Original World Development Indicators extract, including annual historical data and metadata rows. |
| `Region & Income Labels` | Country/economy classifications used to support comparisons. |
| `Combined Data` | Prepared country-level comparison table (2020–2024) with `Income Level`, `Region`, and `Hypothetical Metric`. |
| `Pivot tables` | Original PivotTable summaries for Figures 4A–4C. |
| `Pivot fig 4A` | Additional income-level PivotTable and chart. |
| `Pivot 4B` | Regional 2024 average-enrolment PivotTable. |
| `Pivot 4C` | Hypothetical-category PivotTable for 2022–2024. |
| `4A. Figure A`, `4B. Figure B `, `4C. Figure C ` | Figure-specific presentation sheets. |
| `Dashboard` | Consolidated visual display (contains multiple chart objects). |

### Visualizations

1. **Figure 4A — Income-level comparison:** Compares average primary school enrolment across income groups and years, especially 2021–2024.
2. **Figure 4B — Regional comparison:** Compares average gross enrolment across World Bank regions for 2024 using a bar chart.
3. **Figure 4C — Hypothetical categories:** Compares average gross enrolment across categories A, B, and C for 2022–2024.
4. **Dashboard:** Brings chart views into a single worksheet for easier review.

### Illustrative findings from the saved PivotTable values

- **2024 regional averages:** South Asia is about **113.25%**, and Sub-Saharan Africa about **104.69%**. These are gross enrolment rates, not net enrolment or student counts.
- **2024 income-group averages:** High income **99.23%**; low income **110.01%**; lower middle income **99.02%**; upper middle income **100.35%**.
- Comparisons are descriptive, not causal: years or groups with missing observations may reflect different country samples.

## Workbook 2 — Exercise 2: Basic Visualizations

### Main worksheets

| Sheet | Purpose |
| --- | --- |
| `Data` | World Development Indicators source extract. |
| `Data Cleaned` | Compact, year-based enrolment table with 2020–2025 columns. |
| `1. Introduction` | Introductory charts and tables for comparing average enrolment by income group and improving visual communication. |
| `Introduction rework` | Pivot-based reorganization of introductory enrolment comparisons. |
| `Pivot Table For Data ` | PivotTable summarizing average enrolment across income groups. |
| `2. Organization` | Examples of restructuring category-based data, including male/female/global comparisons, to make charts easier to read. |
| `Organisation rework` | Reorganized age-cohort comparison with a PivotTable and chart. |
| `Stacked bar dstribution` | Stacked-bar view of economy counts by region and income group. |
| `3. Maps` | Country and regional classification data, with map-oriented analysis. |
| `Maps of countries`, `Map of Africa`, `Detail1` | Supporting country/region records and map-related summaries. |

### Visualization objectives

- **Clarity:** Use chronological years, meaningful axis labels, legible legends, and readable scales.
- **Trend analysis:** Compare changes in average enrolment across income groups over time.
- **Composition:** Use stacked bars to communicate how income categories contribute to regional totals.
- **Geographical context:** Organize country and regional fields for geographic comparisons.
- **Storytelling:** Add short insight statements highlighting noteworthy contrasts while distinguishing observations from explanations.

## Data Preparation and Analysis Workflow

1. **Inspect the raw sources.** Identify header rows, indicator code, country/economy identifiers, year columns, and blanks.
2. **Select relevant periods and fields.** Build compact year-wise tables for the chosen analyses.
3. **Match country classifications.** Combine enrolment records with region and income-group metadata; Exercise 1's prepared table includes VLOOKUP-based classification fields.
4. **Review missing values.** Preserve unavailable observations as missing rather than converting them to zero. Confirm that PivotTable averages use numeric observations.
5. **Avoid inappropriate aggregation.** Differentiate country/economy records from World Bank aggregate rows when constructing country-level comparisons.
6. **Summarize with PivotTables.** Use **Average**, rather than **Sum**, for gross enrolment percentages when comparing country observations.
7. **Choose charts by the question.** Columns/bars for group comparisons, lines for temporal trends, stacked bars for composition, and maps for spatial patterns.
8. **Format and review.** Add descriptive titles, units, consistent colours, suitable zero baselines for bars, and validate chart totals against their source PivotTables.

## How to Open and Use the Project

1. Download both `.xlsx` workbooks and open them in **Microsoft Excel Desktop**.
2. In Exercise 1, start at **`Dashboard`** to see the chart collection, then explore **`Combined Data`** and the PivotTable worksheets to trace the numbers.
3. To change a PivotTable, select a cell in it, choose **PivotTable Analyze → Field List**, and adjust rows, columns, filters, or values.
4. To update calculations after source edits, use **Data → Refresh All** (and inspect any lookup errors).
5. In Exercise 2, begin at **`1. Introduction`**, continue to **`2. Organization`**, and explore **`3. Maps`** and related sheets.
6. Check interactive controls in your version of Excel; availability and rendering of PivotCharts, slicers, and map objects can vary across Excel versions and viewers.

## Limitations and Quality Checks

- **Missing observations:** Some country-year enrolment figures are blank. Annual averages may be based on different country subsets.
- **Gross enrolment above 100% is possible:** Do not automatically treat such values as errors.
- **Averages are not population-weighted:** The PivotTable mean of available country values is not the same as the enrolment rate for an entire region.
- **Regional categories differ from continents:** World Bank regions are not a one-to-one continental classification.
- **Hypothetical categories are illustrative:** Do not interpret A/B/C as externally validated metrics.
- **Lookup validation:** Check any formula errors or unmatched country labels in `Combined Data` before making publication-quality claims.
- **Interactive testing:** The workbook contains PivotTables and chart objects. Any intended slicer-to-PivotTable connections should be tested directly in Excel Desktop; their correct operation was not independently verified here.
- **Maps:** Excel map display can depend on version, connectivity, and recognized location names. The supporting worksheets do not in themselves guarantee that a live map chart will render everywhere.

## Tools

- **Microsoft Excel:** data preparation, formulas, PivotTables, PivotCharts, dashboards and chart formatting.
- **World Bank World Development Indicators:** primary-school enrolment statistics and related classifications.

## Project Outcome

The workbooks demonstrate how to prepare public development statistics, aggregate them responsibly, compare patterns across groups and years, and present the results through clearly designed charts and a central dashboard. The exercises emphasize reproducible analysis, interpretable visuals, and awareness of data limitations.
