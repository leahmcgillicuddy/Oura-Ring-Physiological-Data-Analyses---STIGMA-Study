# Oura Ring Physiological Data Analyses - STIGMA-Study

# STIGMA Study — Exploratory Wearables and Menstrual Phase Analysis

This repository contains my ongoing analysis work for the STIGMA Study, a participant-centered menstrual health research project using longitudinal wearable data. The analyses here focus on relationships between menstrual cycle phase and physiological signals captured via the Oura Ring, including sleep, stress, activity, and recovery metrics.

This repo is meant to be a living record of my analytical work in the lab. Files will continue to be added, refined, and extended as new questions are explored and as additional data become available.

# Project Context

The STIGMA Study was designed to address gaps in menstrual health research, particularly the historical exclusion of diverse populations from wearable-based studies. Rather than treating menstrual phase as noise, this work treats it as a meaningful biological context that may shape physiological patterns over time.

My contributions focus on:
	•	Cleaning and structuring longitudinal wearable data
	•	Defining defensible physiological metrics
	•	Exploring phase-level trends and relationships
	•	Stress-testing results with appropriate statistical framing
	•	Identifying limitations and next analytical directions

All analyses are exploratory and hypothesis-generating, not predictive.

# Files
	•	leah_stigma_oura_phase_analysis.ipynb
Core exploratory analysis examining how individual Oura-derived metrics vary across menstrual cycle phases. Includes data filtering logic, phase alignment, visualization, and basic statistical tests.
	•	phase_analysis_sleep_readiness.ipynb
Focused analysis of sleep-related variables and readiness metrics by menstrual phase. Emphasizes physiologically interpretable variables that align closely with Oura’s validated definitions.
	•	stress_sleep_exercise_cycle_regressions.ipynb
Regression-based exploration of relationships between stress, sleep, activity, and menstrual phase variability.
	•	Exploratory Analysis of Stress, Sleep, Activity and Recovery Across Menstrual Phases.pdf
My end of summer term presentation summarizing my motivation, dataset, methods, key findings, limitations, and proposed next steps for this work.

# Methods Overview

Across files, analyses generally follow this pattern:
	1.	Restricting to participants with valid menstrual phase labeling and sufficient wearable coverage
	2.	Aligning daily wearable observations to cycle phase
	3.	Examining single-variable phase differences using appropriate summary statistics
	4.	Exploring variable–variable relationships using correlation and regression
	5.	Testing phase interaction terms where relevant
	6.	Interpreting results conservatively, emphasizing effect sizes and limitations

# Data and Privacy

This repository does not contain raw participant data. Any outputs included here are aggregated, de-identified, or derived. Notebooks have no execution outputs as it is necessary to protect participant privacy.

# Future Directions

This work is ongoing. Planned next steps include:
	•	Expanding per-participant and subgroup analyses, including athlete-only cohorts and groups with consistently longer average cycle lengths
	•	Updating and integrating background survey data (age, BMI) using the most recent weekly and baseline files to improve covariate control
	•	Increasing sample size where possible by resolving missing or uncleaned weekly survey files and clarifying inclusion criteria (e.g., required cycle length fields)
	•	Refining how exercise is quantified by testing multiple activity variables, accounting for non-wear time, removing extreme outliers, and exploring composite exercise metrics
	•	Extending regression analyses with improved visualization, non-linear models, and phase- or cohort-specific fits
	•	Comparing cycle length variability within and across cohorts, including cohort-level averages and within-person variability across cycles
	•	Exploring relationships between lifestyle factors (stress, sleep, activity) and cycle length variability, with each cycle treated as a distinct observation where appropriate

# Acknowledgements

This work was completed as part of the STIGMA Study with mentorship and guidance from the Engelhardt Lab and the broader STIGMA research team. I am deeply grateful to the participants who contributed their time and data to this study.
