# Dancing with the Stars: Data Analytics Project

## Project Overview

This project explores historical data from *Dancing with the Stars (DWTS)* to investigate how judges' scores, celebrity backgrounds, and other factors relate to contestants' success in the competition.

Using Python and statistical analysis, I aim to identify patterns across seasons and examine whether judges' evaluations align with final competition outcomes.

## Research Questions

1. How strongly do judges' scores correlate with contestants' final placements?
2. How often does the highest-scoring contestant win the competition?
3. Is there an association between a celebrity's professional background and their likelihood of finishing in the top three?
4. Which contestants and seasons show the largest differences between judges' scoring rankings and final placements?

## Dataset

The project uses historical DWTS contestant information and weekly judges' scores across Seasons 1–34.

The dataset includes contestant names, professional dance partners, celebrity industries, final placements, and weekly judges' scores.

**Source:** 2026 Mathematical Contest in Modeling (MCM), Problem C dataset.

## Tools and Technologies

- **Python:** Data cleaning, manipulation, and analysis
- **Pandas:** Data transformation and aggregation
- **SciPy:** Statistical hypothesis testing
- **Matplotlib:** Data visualization
- **Jupyter Notebook / VS Code:** Analysis and documentation
- **Tableau:** Planned interactive dashboard

## Statistical Methods

### Spearman's Rank Correlation

Used to evaluate the relationship between judges' scoring rankings and contestants' final placements across individual seasons.

### Chi-Square Test of Independence

Used to investigate whether celebrity industry is associated with finishing in the top three.

### Cramér's V

Used to measure the strength of association between celebrity industry and top-three placement.

## Preliminary Findings

- Judges' scoring rankings and final placements were positively correlated across all 34 seasons.
- In the initial analysis, the highest-scoring contestant did not win in 20 of 34 seasons.
- Season 27 was a notable example: Bobby Bones won despite ranking eighth in average judges' scores.
- The Chi-Square test did not find a statistically significant association between celebrity industry and top-three placement (p = 0.7921).
- Athletes had the highest observed top-three finish rate (28.42%) among the five industry groups analyzed.

These findings are preliminary and will be revisited as the analysis develops.

## Project Structure

- `data/` — Original and processed datasets
- `notebooks/` — Python analysis notebooks
- `sql/` — SQL queries for future analysis
- `visualizations/` — Charts and visualizations

## Project Status

**In Progress**

Future work includes additional exploratory analysis, visualizations, and an interactive Tableau dashboard.