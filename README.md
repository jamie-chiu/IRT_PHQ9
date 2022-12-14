# An item response theory analysis of the Patient Health Questionnaire

The 9-item Patient Health Questionnaire (PHQ-9) is a commonly-used depression measurement tool. The ratings on each question is often treated as continuous, summed to a total score, and then compared against different cut-offs to determine a respondent's depression severity. However, the PHQ-9 is an ordinal scale where each question has four rank-ordered responses - "Not at all", "Several days", "More than half the days", and "Almost every day".  

The following report is an exploration of using an ordinal-appropriate model to analyse the PHQ-9. More specifically, the Graded Response Model from Item Response Theory is applied to examine the psychometric properties of the PHQ-9. The data comprises 2,177 responses to the PHQ-9, gathered from two open data sets. Overall, most of the items of the PHQ-9 has adequate discrimination and difficulty. Item 9 performed the worst, even participants with high depression did not always endorse it. Item 9 may be indicative of a related but separate latent trait instead of depression, and could be potentially excluded from the Patient Health Questionnaire.  

All analyses were carried out in R and the data and code are provided for reproducibility.  

<br />

## Contents of this Repo:  
- csv file of PHQ-9 data used for analyses
- r markdown file of the report, including all code necessary to reproduce analyses
- PDF output of the paper in APA format
- copy of the PHQ-9 rating scale for reference  

Author: Jamie C. Chiu

<br />
<br />

---

<br />

### R packages used:

All data analyses were conducted using R (Version 4.2.1; R Core Team, 2022) and theR-packages:
- car(Version 3.1.1; Fox & Weisberg, 2019; Fox, Weisberg, & Price, 2022),
- carData(Version 3.0.5; Fox et al., 2022),
- citr(Version 0.3.2; Aust, 2019),
- corrplot2021(Wei & Simko, 2021),
- dplyr(Version 1.0.10; Wickham, François, Henry, & Müller, 2022),
- factoextra(Version 1.0.7; Kassambara & Mundt, 2020),
- FactoMineR(Version 2.6; Lê et al.,2008),
- forcats(Version 0.5.2; Wickham, 2022a),
- ggplot2(Version 3.3.6; Wickham, 2016),
- lavaan(Version 0.6.12; Rosseel, 2012),
- ltm(Version 1.2.0; Rizopoulos, 2006),
- MASS(Version 7.3.57; Venables & Ripley, 2002),
- mokken(Version 3.0.6; Van der Ark, 2007,2012),
- msm(Version 1.7; Jackson, 2011),
- papaja(Version 0.1.1; Aust & Barth, 2022),
- poLCA(Version 1.6.0.1; Linzer & Lewis, 2011),
- polycor(Version 0.8.1; Fox, 2022),
- psych(Version 2.2.9; Revelle, 2022),
- purrr(Version 0.3.5; Henry & Wickham, 2022),
- readr(Version 2.1.3; Wickham, Hester, & Bryan, 2022),
- scatterplot3d(Version 0.3.42; Ligges &Mächler, 2003),
- stringr(Version 1.5.0; Wickham, 2022b),
- tibble(Version 3.1.8; Müller &Wickham, 2022),
- tidyr(Version 1.2.1; Wickham & Girlich, 2022),
- tidyverse(Version 1.3.2;Wickham et al., 2019), and
- tinylabels(Version 0.2.3; Barth, 2022).

