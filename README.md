# Dancing with the Stars: Data Analytics Project

## Project Overview

This project explores historical data from *Dancing with the Stars (DWTS)* to examine how judges' scores, celebrity backgrounds, professional dance partners, and competition performance relate to contestants' overall success.

Using Python, statistical analysis, and data visualization, I investigated patterns across 34 seasons to better understand what contributes to a contestant's success and where judges' evaluations differ from final competition outcomes.

The goal of this project was to go beyond identifying winners and explore the relationships between scoring, experience, and competition survival.

## Research Questions

1. How strongly do judges' scores correlate with contestants' final placements?
2. How often does the highest-scoring contestant win the competition?
3. Is there a relationship between celebrity professional background and competition success?
4. Does a professional dance partner's experience relate to their success rate?
5. How do judges' scores relate to the percentage of a season a contestant completes?
6. Can early-season performance help explain how long contestants remain in the competition?

## Dataset

This project uses the *2026 Mathematical Contest in Modeling (MCM) Problem C: Data With The Stars* dataset, published by COMAP.

The dataset contains contestant information, competition results, and weekly judges' scores from Seasons 1–34 of *Dancing with the Stars*.

**Source:** [COMAP — 2026 MCM Problems](https://contest.comap.com/undergraduate/contests/mcm/contests/2026/problems/index.html)

The original dataset is not included in this repository. To reproduce the analysis:

1. Visit the official COMAP source linked above.
2. Download the Problem C CSV dataset.
3. Create a `data/raw/` directory in the project if it does not already exist.
4. Save the file as `2026_MCM_Problem_C_Data.csv` inside that directory.
5. Open and run `notebooks/notebook.ipynb` from the notebook's directory.

The analysis and interpretations presented in this project are my own independent work.

## Tools and Technologies

- **Python:** Data cleaning, transformation, and exploratory analysis
- **Pandas and NumPy:** Data manipulation and calculations
- **SciPy:** Statistical hypothesis testing and correlation analysis
- **Matplotlib:** Data visualization
- **Jupyter Notebook / VS Code:** Analysis development and documentation
- **Git and GitHub:** Version control and project management

## Methodology

The analysis began with exploring and cleaning the original dataset, including handling missing values, restructuring weekly judges' scores, and standardizing contestant and professional partner information.

I then used several statistical methods to investigate relationships between different competition factors:

- **Spearman's Rank Correlation:** Examined the relationship between judges' scoring rankings and final placements.
- **Chi-Square Test of Independence:** Tested whether celebrity industry was associated with top-three placement.
- **Cramér's V:** Measured the strength of the association between celebrity industry and top-three placement.
- **Pearson Correlation:** Examined relationships involving professional dance partner experience, judges' scores, and competition survival.
- **Exploratory Visualizations:** Used charts to identify patterns, distributions, and exceptions across seasons.

Because DWTS seasons vary in length, I also calculated the percentage of scored weeks each contestant completed to make comparisons across seasons more consistent.

## Key Findings

### Judges' Scores and Final Placements

Judges' scoring rankings were positively associated with contestants' final placements across the seasons analyzed. However, the highest-scoring contestant did not always win.

In 20 of the 34 seasons, the contestant with the highest average judges' score was not the eventual winner.

Season 27 was a particularly notable example, with Bobby Bones winning despite ranking eighth in average judges' scores. This highlights how competition outcomes can differ from judges' evaluations.

### Celebrity Background and Competition Success

Athletes had the highest observed top-three finish rate among the five celebrity industry groups analyzed, at approximately 28.42%.

However, the Chi-Square test did not identify a statistically significant relationship between celebrity industry and top-three placement (p = 0.7921).

This suggests that the observed differences between industries were not strong enough to establish a statistically significant association in this dataset.

### Professional Dance Partner Experience

Professional dance partner experience showed a moderate positive correlation with overall win rate (r = 0.4251).

However, when examining professionals with at least five appearances, this relationship became much weaker (r = 0.0964).

These findings suggest that having more appearances does not necessarily translate into a higher win rate among experienced professionals.

### Judges' Scores and Competition Survival

Contestants with higher average season judges' scores generally remained in the competition longer.

The analysis found a strong positive correlation between average season scores and the percentage of the competition completed (r = 0.836).

However, because contestants who remain longer have more opportunities to improve their scores, this relationship should not be interpreted as proof that higher scores cause longer survival.

## Limitations

Several factors should be considered when interpreting these findings.

- Audience voting plays an important role in competition outcomes, but complete individual voting data was not available.
- Competition formats, season lengths, and judging panels have changed over time.
- Some professional dance partners appeared substantially more often than others, affecting comparisons of experience and success.
- Correlations identify relationships between variables but do not establish causation.

These limitations are important when comparing contestants across different seasons and interpreting the factors associated with competition success.

## Project Structure

```text
dwts-data-analysis/
├── notebooks/
│   └── notebook.ipynb
├── README.md
└── .gitignore
```

The analysis uses a local `data/raw/` directory for the original CSV, which is excluded from version control.

## Project Status

**Python Analysis: Complete**

The data cleaning, exploratory analysis, statistical testing, and written interpretations have been completed. The notebook has been successfully executed from a restarted kernel without errors.

**Next Phase: Tableau Dashboard**

The next phase will focus on creating an interactive Tableau dashboard to communicate the most important findings visually, including judges' scores, contestant outcomes, and professional dance partner performance.

## Conclusion

This project demonstrates how data analysis can uncover patterns in competition outcomes while also highlighting the limitations of relying on any single measure of success.

Although judges' scores, professional dance partner experience, and other factors showed relationships with competition performance, the results also revealed notable exceptions.

Overall, the project strengthened my experience with Python, data cleaning, statistical analysis, data visualization, and communicating findings through a complete analytical workflow.