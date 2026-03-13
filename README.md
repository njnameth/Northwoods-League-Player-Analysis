# Northwoods League Player Analysis

# Project Overview
This project analyzes offensive data from the Northwoods League (NWL) to determine which "process" statistics (like Walk Rate and Isolated Power) most effectively correlate with "results" metrics like Runs Created (RC) and On-base Plus Slugging (OPS).

The goal is to move beyond traditional counting stats (Hits, Home Runs) and identify the underlying plate discipline and power profiles that define elite collegiate hitters.

# Key Insights
Strongest Predictors: Beyond standard results metrics, Slugging Percentage (SLG) and Isolated Power (ISOP) showed the highest correlation with high-value offensive output.

Plate Discipline: The analysis explores the relationship between BB/K ratios and offensive efficiency, identifying players who maximize productivity through disciplined hitting.

Performance Tiers: By comparing "Qualifiers" (players meeting a minimum Plate Appearance threshold) against the full league, the project highlights the sustainability of top-tier performance with a viable sample size. 

# Data & Methodology
The Dataset
Source: Scraped/Downloaded from Baseball Reference data.

Scope: 778 players across the league, with a subset of 82 "Qualified" hitters. A minimum of 50 AB's while producing 2.7 AB's per games played is the cutoff. 

Features: Includes advanced metrics such as SECA (Secondary Average), RC (Runs Created), ISOP (Isolated Power), and BB/K (Walk-to-Strikeout ratio).

# Technical Workflow
Data Cleaning: Handled multi-indexed headers from Excel exports, converted "Object" types to numeric formats, and isolated player-specific identifying data.

Feature Engineering: Calculated custom performance metrics including Strikeout Percentage (K_pct) and Walk Percentage (BB_pct) to normalize performance against Plate Appearances.

Correlation Analysis: Developed a correlation matrix to rank "process stats" against team-value metrics like Runs Created.

Visualizations: Created Seaborn-based bar and scatter plots to visualize the statistical drivers of offensive success. 

# File Descriptions
NWL_Poster.ipynb: The primary analysis engine containing data cleaning, EDA, and visualization code.

2025_NWL_Stats.xls: Raw data source containing league-wide hitting statistics.

nwl_feature_importance.png: Exported visualization showing the impact of various stats on run production.

# Conclusion
This project was conducted in preperation for our semester long capstone project. The intention is for team Northwoods League Teams to use these findings to inform scouting decisions regarding emerging college talent. By revealing which of the advanced metrics actually matter, teams should be able to focus on the key areas identified in our study (ISOP vs. BB/K.) 
