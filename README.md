# Health-Based Clustering of Turkish Provinces

## Overview

This project explores regional health-related patterns among the 81 provinces of Türkiye using public data obtained from TÜİK (Turkish Statistical Institute).

The study is inspired by the article *Analysis of City Demographics in Türkiye Using Data Mining Techniques* by Doğuç, Şahinbaş, and Silahtaroğlu (2023). Rather than reproducing the original study, this project presents a health-focused partial replication and methodological extension using a smaller subset of health-related indicators.

## Dataset

The analysis uses five health-related indicators:

* Infant Mortality Rate
* Life Expectancy at Birth
* Applications per Doctor
* Health Satisfaction Rate
* Public Health Service Satisfaction Rate

The data originates from TÜİK's provincial well-being indicators dataset.

## Methods

The following techniques were applied:

* Data Cleaning and Preparation
* Feature Standardization
* K-Means Clustering
* Principal Component Analysis (PCA)
* Fuzzy C-Means Clustering

## Key Findings

* Three distinct health-related provincial profiles were identified.
* Cluster characteristics differed across mortality, life expectancy, healthcare utilization, and satisfaction indicators.
* PCA revealed visible separation among clusters and highlighted provinces with distinctive profiles.
* Fuzzy C-Means showed that some provinces exhibit mixed characteristics and cannot be assigned confidently to a single cluster.
* A major eastern and southeastern regional pattern reported in the reference study also appeared in this analysis.

## Repository Contents

* `health_clustering_analysis_turkiye.ipynb` – Complete Jupyter Notebook
* `health_clustering_analysis_turkiye.html` – Exported notebook version
* `requirements.txt` – Required Python packages

## Author

**Daniyal Hemmati**
Management Information Systems (MIS)
Istanbul Medipol University

## Reference

Doğuç, Ö., Şahinbaş, K., & Silahtaroğlu, G. (2023). *Analysis of City Demographics in Türkiye Using Data Mining Techniques.*
