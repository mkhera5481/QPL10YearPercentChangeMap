## Queens Public Library (QPL) — 10-Year Percent-Change Choropleth Maps

*2013 → 2023 American Community Survey (ACS) comparison*

-----------------------------------------------------------------------

### 📂 How to access the interactive maps

1. **Download the repo files**

   * Click the green **“Code”** button (upper-right on the repo page).
   * Choose **Download ZIP**.
   * Un-zip the file anywhere on your computer (all contents must stay in **one folder**).

2. **Open each map**

   * Inside the un-zipped folder you’ll find **`index1.html`**, **`index2.html`**, and **`index3.html`**.
   * Double-click any of them to launch the interactive Leaflet map in your default browser (no extra software needed).

> **Why three files?**
> A single self-contained HTML map exceeded GitHub’s 25 MB file limit (\~65 MB). Splitting the variables into three smaller maps keeps each file under the limit while preserving full interactivity.

-----------------------------------------------------------------------

### 🗺️ What each map contains

| HTML file       | Variable themes                                                                          | Typical use                                                                        |
| --------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| **index1.html** | **Sex & Age-group demographics**  (`SEX_*`, `AGE_*`)                                     | View percent change for male/female shares and eleven 5-year age cohorts.          |
| **index2.html** | **Nativity, Race / Ethnicity, Language**  (`BIRTHPLACE_*`, `RACE_*`, `LANGUAGE_SPANISH`) | Explore shifts in birthplace composition, racial/ethnic mix, and Spanish speakers. |
| **index3.html** | **Household, Housing, Income**  (`HOUSEHOLD_*`, `HOUSING_*`, `INCOME_*`)                 | Compare changes in household size, tenure, housing stock, and income brackets.     |

*(Five variables with very sparse data were dropped to keep file size down: `LANGUAGE_ASIAN_ISLANDER`, `LANGUAGE_INDO_EUROPEAN`, `LANGUAGE_UNSPECIFIED_OTHER`, `LANGUAGE_LIMITED_ENGLISH`, and `RACE_PACIFIC_ISLANDER`.)*

-----------------------------------------------------------------------
### 🖱️ How to use the map interface

* **Variable list:** A box on the **right-hand side** lists the variables available in that map.

  * ✅ **Select exactly one variable at a time** (checkbox).
  * 🔄 Before picking another, un-tick the current one to clear the view.
* **Color scale (legend at bottom-left):**

  * **Dark green = −100 %** (largest decrease)
  * **White = 0 %** (no change)
  * **Dark purple = 300 % +** (largest increase)
  * **Yellow = No data** for that branch’s service area.
* **Pop-ups:** Click any polygon (branch service area) to see:

  * Branch name
  * Exact 10-year percent change for the currently selected variable.

-----------------------------------------------------------------------

### 🔍 What the maps represent

* **Geography:** Polygons outline the QPL branch *service areas* (not just the branch buildings).
* **Metric:** Each variable shows the **percent change from 2013 to 2023** using ACS 5-year estimates (2011–2013 vs. 2021–2023).
* **Interpretation:**

  * Deep-purple polygons highlight branches where the metric surged (e.g., income doubled or senior population grew > 100 %).
  * Deep-green polygons mark sharp declines (e.g., under-5 population dropped by half).
  * Hovering turns borders white for quick visual focus.

These interactive maps let staff and researchers pinpoint where demographic transformations are occurring across Queens and support data-driven outreach, programming, and resource allocation for the next strategic cycle.

-----------------------------------------------------------------------

**Enjoy exploring!**
Questions or suggestions? Open an issue or pull-request on this repo.
