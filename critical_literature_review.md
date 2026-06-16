# Clustering Turkish Provinces Using Data Mining: A Focused Literature Review and Project Comparison

**Author:** Daniyal Hemmati
**Affiliation:** Department of Management Information Systems, Istanbul Medipol University
**Date:** June 2026

## Introduction

Data mining techniques provide useful tools for identifying similarities and differences among regions based on large collections of social, economic, demographic, and public-service indicators. In Türkiye, province-level data published by the Turkish Statistical Institute (TÜİK) has supported research into regional development, quality of life, healthcare, transportation, tourism, and socioeconomic inequality.

This focused literature review evaluates the study *Analysis of City Demographics in Turkiye Using Data Mining Techniques* by Doğuç, Şahinbaş, and Silahtaroğlu (2023). The article is particularly relevant because it applies clustering techniques to a broad provincial dataset and investigates how Türkiye’s 81 provinces can be grouped according to shared characteristics.

The review first places the article within earlier province-level clustering research, then examines its data, methodology, findings, strengths, and limitations. Finally, it compares the article with my health-related clustering project, which was developed as a partial replication and methodological extension.

## Background Literature

Previous studies have applied clustering methods to different dimensions of Turkish provincial development. As summarized by Doğuç et al. (2023), this literature generally focused on narrower groups of variables than their study.

Bulut (2019) examined provincial life-satisfaction indicators using Expectation Maximization and K-Means. The study identified a regional pattern in which many eastern and southeastern provinces appeared together, suggesting that differences in life satisfaction were connected to broader regional inequalities.

Yılancı (2010) used fuzzy clustering and K-Means to classify provinces according to socioeconomic indicators, including unemployment, education, public investment, population per physician, and infant mortality. The results produced broad developed and underdeveloped provincial groups.

İncekırık and Altın (2021) focused on transportation statistics and found differences between provinces with developed transportation and trade activity and those with more limited infrastructure. Tekin (2015) examined 16 health indicators and reported substantial differences between eastern and western provinces in the quality of health services. Kandemir (2018), meanwhile, used accommodation and tourism statistics and found that major destinations such as Ankara, Antalya, and İstanbul displayed distinctive clustering characteristics.

Together, these studies demonstrate that provincial clustering in Türkiye consistently reveals regional differences. However, most earlier studies were limited to a single field, such as health, transportation, tourism, socioeconomic development, or satisfaction.

## Review of the Focal Study

Doğuç et al. (2023) sought to provide a broader demographic analysis than previous studies. Their purpose was to identify similarities and differences among Türkiye’s provinces and to evaluate how these patterns might support public investment, budgeting, and regional planning.

The authors assembled TÜİK data covering the period from 2015 to 2020. The dataset contained 142 variables drawn from 23 source categories, including education, demography, health, transportation, environment, employment, income, security, tourism, culture, infrastructure, and happiness.

The study first conducted an overall clustering analysis using all 142 variables. It then reorganized the data into seven thematic perspectives, producing eight analyses in total:

1. Overall demographic characteristics
2. Education
3. Population and settlement
4. Livelihood, income, and purchasing power
5. Health
6. Satisfaction
7. Security
8. Cultural opportunities and utilization

The main analytical method was an enhanced form of Fuzzy C-Means clustering. Unlike K-Means, which places each observation into one fixed group, Fuzzy C-Means allows provinces to have different degrees of membership across clusters. The authors tested different numbers of clusters and used measures such as the Xie–Beni Index, Partition Entropy, and Partition Coefficient to select the preferred solution for each analytical perspective.

The resulting clusters were displayed on provincial maps, allowing the reader to observe both statistical and geographic patterns.

## Main Findings

The general analysis using all 142 variables produced nine clusters. İstanbul, Ankara, İzmir, and Konya appeared as individual clusters, indicating that their demographic structures differed substantially from those of other provinces.

Across the thematic analyses, the authors identified three recurring patterns.

First, major metropolitan provinces frequently differed from the rest of Türkiye. İstanbul, Ankara, and İzmir were often isolated or grouped separately, particularly in population, culture, security, and overall demographic characteristics.

Second, the analyses repeatedly showed distinctions between eastern and western provinces. This pattern was especially visible in health, security, purchasing power, education, and satisfaction.

Third, the authors argued that large provinces may influence nearby smaller provinces by providing access to universities, hospitals, employment, cultural activities, and other services. Smaller provinces located near major urban centers sometimes showed similarities with their larger neighbors, while geographically isolated provinces were more likely to cluster with other small or less-developed provinces.

The health-services analysis is particularly relevant to my project. It produced six clusters, including a group composed of 15 mainly eastern and southeastern provinces:

Adıyaman, Ağrı, Batman, Bingöl, Bitlis, Gaziantep, Hakkâri, Hatay, Iğdır, Mardin, Muş, Siirt, Van, Şanlıurfa, and Şırnak.

The authors interpreted this grouping as evidence of differences between eastern and western Türkiye in access to health services, healthcare infrastructure, and health standards.

## Strengths of the Study

One of the study’s main strengths is its broad scope. The use of 142 variables allows provincial similarities to be examined from several perspectives rather than through one isolated category.

A second strength is the inclusion of all 81 provinces. This provides national coverage and makes the findings relevant to regional policy and public planning.

The use of Fuzzy C-Means is also appropriate because provinces may share characteristics with multiple groups. Regional profiles are rarely completely separate, and fuzzy clustering represents this uncertainty more realistically than a method that forces every province into a single fixed category.

Another strength is the use of several cluster-validity measures when selecting the number of clusters. This is more rigorous than choosing the number of clusters without testing alternatives.

Finally, the provincial maps make the findings accessible and reveal geographic relationships that may be difficult to recognize from tables alone.

## Limitations and Critical Evaluation

Despite its contribution, the study has several limitations.

First, the dataset is historical. Because it covers 2015–2020, its results should not automatically be interpreted as representing present-day conditions.

Second, the inclusion of 142 variables creates a comprehensive dataset but also makes interpretation difficult. When many indicators are included simultaneously, it may be challenging to determine which variables are primarily responsible for the formation of each cluster.

Third, the article provides less detail about data cleaning, missing-value treatment, standardization, and reproducibility than would be desirable for someone attempting to reconstruct the complete analysis.

Fourth, clustering is descriptive rather than causal. The results can show that provinces are similar, but they cannot prove why those similarities exist. For example, the suggestion that large cities directly influence neighboring provinces is plausible, but this relationship would require additional spatial or causal analysis.

Fifth, the number and composition of clusters change across analytical perspectives. Although this is expected, it makes direct comparison between categories more complex.

Finally, the study provides strong visual and descriptive findings but does not test whether its cluster assignments remain stable under alternative algorithms or data samples.

## Comparison with My Project

My project, *Health-Based Clustering of Turkish Provinces*, was inspired by Doğuç et al. (2023), but it is not a complete reproduction of their research. It is more accurately described as a health-focused partial replication and methodological extension.

The original study used 142 variables from multiple demographic domains. My project uses five health-related indicators:

* Infant mortality rate
* Life expectancy at birth
* Applications per doctor
* Health satisfaction rate
* Public-health-service satisfaction rate

A technical distinction is important. In the original article, infant mortality and life expectancy are categorized under Demography, while the remaining three indicators are categorized under Health. Therefore, my project uses the term **health-related indicators** rather than claiming to reproduce the article’s exact health category.

The original article mainly relied on enhanced Fuzzy C-Means clustering and selected different cluster counts using validity indices. My project applied three complementary methods:

* K-Means for hard cluster assignments
* Principal Component Analysis for two-dimensional visualization
* Standard Fuzzy C-Means for overlapping membership analysis

The project also included standardized cluster heatmaps, PCA labeling of recognizable and unusual provinces, membership-degree tables, and identification of ambiguous provinces.

A notable similarity appeared when the results were compared. All 15 provinces in the eastern and southeastern health-services cluster reported by Doğuç et al. were also placed together in one of my K-Means clusters. However, my cluster contained additional provinces, meaning that the solutions were similar but not identical.

This result provides evidence that a major regional pattern identified in the original article remains visible even when a smaller variable set and a different clustering design are used.

The two works therefore have complementary strengths. The original article is stronger in breadth, geographic mapping, and cluster-number selection. My project is narrower but provides a more transparent and focused workflow, including standardization, PCA visualization, cluster-profile interpretation, and fuzzy-membership analysis.

## Research Gap and Future Directions

The literature demonstrates that regional differences in Türkiye can be identified using clustering, but several opportunities remain for further research.

Future studies could:

* Use updated province-level health data
* Compare changes in provincial clusters across time
* Apply spatial clustering methods that consider neighboring provinces directly
* Test cluster stability using several algorithms
* Examine which variables contribute most strongly to each cluster
* Combine healthcare indicators with income, education, infrastructure, and migration
* Use causal or spatial analysis to test whether major cities influence surrounding provinces
* Reconstruct the full health-related analysis using the original article’s variables and cluster-validity procedures

These extensions would move the research from descriptive grouping toward a deeper explanation of regional inequality.

## Conclusion

Doğuç et al. (2023) make an important contribution to province-level data analytics in Türkiye by examining all 81 provinces through a broad set of 142 demographic variables. Their use of Fuzzy C-Means and multiple analytical perspectives reveals recurring differences between metropolitan and non-metropolitan provinces, eastern and western regions, and provinces with different levels of access to services.

The study is especially valuable because it demonstrates how public statistical data can support regional planning and investment decisions. At the same time, its historical dataset, descriptive design, and limited reproducibility details leave room for focused extensions.

My project builds on this foundation by narrowing the analysis to five health-related indicators and adding K-Means, PCA, standardized cluster profiles, and fuzzy-membership interpretation. The strong overlap between the eastern and southeastern grouping in both analyses suggests that the original article identified a meaningful regional pattern that remains visible under a smaller and methodologically different model.

Overall, the article and the project together demonstrate the value of data mining for examining regional health and demographic differences across Türkiye.

## Reference

Doğuç, Ö., Şahinbaş, K., & Silahtaroğlu, G. (2023). *Analysis of city demographics in Turkiye using data mining techniques*. **Acta Infologica, 7**(1), 107–123. https://doi.org/10.26650/acin.1132510
