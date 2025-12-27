# 180-day-data-roadmap
Journey to Data Analyst
Goal : Finding which Genres netflix should invest in? 
Which country should Netflix invest in more?
Is there a trend over time (Year vs Count)
Are there any missing values, that will break my analysis
The granularity of this dataset is one movie/TV show title per row.
# 180-Day Data Analyst Journey

## Day 2: Data Exploration (Netflix Dataset)

- **Granularity:** One unique title per row.
- **Null Audit:** - `Director` column: ~30% missing data.
  - `Cast` column: ~10% missing data.
- **Data Types:**
  - Qualitative: `title`, `type` (Movie/TV Show).
  - Quantitative: `release_year`.
  - Categorical: `rating` (TV-MA, PG-13).
  ### Spot Check Findings:
- **Categories:** Confirmed only 'Movie' and 'TV Show' exist (No typos found).
- **Gaps:** Observed a massive spike in content starting around 2015, with very sparse data pre-1980.
- **Anomalies:** Found 3 lines with Ratings listed as mins.
## Day 3: Pivot Table Foundations
- **Analysis:** Compared the volume of Movies vs. TV Shows.
- **Key Finding:** Netflix has significantly more Movies than TV Shows (approx. 2:1 ratio).
- **Tool Used:** Excel Pivot Tables (Rows: Type, Values: Count of Title).
- **Data Quality Note:** Found that some release years have very few entries, suggesting the dataset might be truncated or filtered.
## Day 4: Market & Content Strategy Analysis
- **Top Markets:** Identified USA, India, and UK as the primary content producers.
- **Content Personality:** - **India:** Strongly skewed toward TV-14 (General Audience).
    - **USA/UK:** Heavy focus on TV-MA (Mature/Adult) content.
- **Visuals:** Created a Stacked Bar Chart to compare rating distributions across top countries.
- **Business Insight:** If Netflix wants to expand into the "Family" market in the UK, there is a clear content gap compared to the US library.
## Day 5: Data Categorization & Consolidation
- **Technique:** Used Pivot Table "Manual Grouping" to simplify 14 ratings into 3 categories (Family, Teen, Adult).
- **Metric Shift:** Converted raw counts to '% of Column Total' to see the relative share of content types.
- **Discovery:** In the US market, 'Adult' content accounts for X% of the library, while 'Family' content is only Y%.
- **Skill:** Learned to handle categorical data without complex nested IF statements.
