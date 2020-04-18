# Data Science Methods Utilized to Predict Maternal and Neonatal Care in Sub-Saharan Africa

By: Suditi Shyamsunder

April 17, 2020 

## Introduction
Throughout the world, there are insufficient health care practices and facilities for mothers and their newborns. The first week of life is a particularly vulnerable time and 73% of neonatal deaths occur during this period [2]. In developing nations in Sub-Saharan Africa, the quality of newborn and maternal care needs to be improved and standardized. A study that analyzed Gallup World Poll data found that in comparison to other regions of the world, sub-Saharan Africa has the lowest ratings for well-being and the lowest satisfaction with health care [4] Right now, newborn care practices are not up to par because resources are not being distributed where they need to be. In fact, according to another study that looked at antenatal care practices on the survival rates of newborns in Sub-Saharan Africa, utilization of at least one antenatal care visit by a skilled provider during pregnancy reduced the risk of neonatal mortality by 39% in countries within this region [3]. More health care facilities are required in rural parts of Africa and knowledge of newer practices that have been proven to save more lives need to be spread to health care providers throughout the continent. Every year, 2.9 million neonates die and saving even some of these lives is a meaningful pursuit [2].

The first data science method analyzed in this paper is Bayesian Hierarchical Regression Modeling approach. This method was utilized in an article aiming to discover the distribution of adolescent first births in Sub-Saharan Africa. Research papers such as this one discover where the demand is highest for improved health and education efforts within the Sub-Saharan region. Another data science technique that will be discussed is correlation analysis combined with GIS mapping techniques. This method was utilized by a paper that analyzed subnational inequalities in healthcare throughout Tanzania. The results of this research were able to be visualized and summarized through data science GIS mapping techniques. Overall, the central research question focused on in this paper is how are geospatial data science methods utilized to predict and understand the inequalities and insufficiencies in neonatal and maternal health care practices throughout Sub-Saharan Africa. 

## Inquiry Type 
The type of inquiry that is being attempted to answer is both an exploratory and explanatory inquiry. Exploratory questions generally aim to understand what is happening regarding a particular process or system. On the other hand, explanatory inquiries work to understand a situation by digging into its causes and effects. In this paper, the research strives to understand the realities of health care for neonates and mothers in Sub-Saharan Africa as well as what causes inequalities and insufficiencies in the system. This broad idea can also be broken down into many sub-questions. 

One specific sub-question that can be addressed from the broader topic is where throughout Sub-Saharan Africa are inequalities most prevalent? In addition, where are resources the most lacking, and where is the need for improvement of health care the highest? These exploratory questions seek to understand the current situation so that it can be assessed and change can be targeted where it would be most effective. One explanatory sub-questions that can be addressed under the broader question posed earlier is what are some predictors or causes of poor maternal and neonatal care throughout Sub-Saharan Africa. This question seeks to understand what specific practices and situations are most responsible for the inequalities that we see.  

## Methods

### Method 1
The first data science method being addressed in this paper is the Bayesian Hierarchical Regression Modeling technique. This method was utilized by a paper striving to understand the distribution of adolescent first births within three African countries: Uganda, Kenya, and Tanzania. This study utilized Demographic and Health Surveys (DHS), and the researchers analyzed the data from first births before the age of 20. They also disaggregated it into three groups: under 16, 16-17, and 18-19 years of age. Using this data combined with GPS-located cluster data and adaptive bandwidth kernel density estimates, they were able to create descriptive choropleths, and prevalence maps. In addition, they employed kernel density estimation (KDE) in order to create heatmaps. 

The researchers utilized a Bayesian hierarchical regression modeling approach to map adolescent first birth at a district level with estimates of uncertainty. A Bayesian hierarchical regression model is a statistical model that allows data scientists to make conclusions about their data using Bayes Theorem, shown below. 

[Bayes]( https://suditishyamsunder.github.io/workshop/Bayes) 

More specifically, in order to map adolescent first births with estimates of uncertainty, they employed an Integrated Nested Laplace Approximation (INLA) technique. The INLA modelling approach is particularly useful for small area estimation. This technique was utilized using the INLA package in R, and it uses a Bayesian hierarchical spatial regression model. The ability to estimate uncertainties is particularly useful for discovering where future data may need to be collected. Below is a map from the paper that shows the uncertainty of their data based on the calculations from the Bayesian hierarchical regression model [5]. 


### Method 2
The second data science technique being discussed in this paper is correlation analysis combined with GIS mapping techniques. This method was utilized by a paper that analyzed subnational inequalities in healthcare throughout Tanzania. The authors attempted to discover the distribution of healthcare inequalities as well as what was causing them. In their analyses, they utilized primarily census data, as well as some DHS data. They looked at indicators such as GDP, proportion of women with a certain level of education, total fertility rate, and number of live births. They performed bivariate correlation analyses using Stata 13.1, and considered anything with above .8 as the correlation coefficient to be a very strong association. 

They also utilized geographical information system (GIS) mapping in order to visualize their results and better see the subnational variations in care at birth for women across Tanzania. They generated Choropleth and proportional maps with ArcGIS 10.3 software. They mapped subnational variations in rural birth density, births by rural women in a health facility, births by rural women by C-section, per capita recurrent expenditure, health workforce density, health facility density, and health facilities availability of tracer drugs. Below are subnational maps of coverage of care at birth for rural women in Tanzania compared to financial inputs. The first maps births by rural women in a health facility, and the second maps births by rural women by Caesarean section [1]. 


## Conclusion
While it is essential to understand the distribution of potential mothers as well as health care facilities, I feel there is a gap in the literature. It would be interesting to see whether or not the distribution of the need, in this case pregnant mothers, is aligned with the distribution of supply, in this case facilities. 
It would be beneficial to research the distance that mothers need to travel in order to get access to a facility to give birth in. This research would allow us to see the distribution and any inequality that exists in different parts of Sub-Saharan Africa. It is possible that the facilities with the best care are concentrated in the more wealthy areas, and it is important to be able to see this distribution. With this information, policy makers may be more likely to know where money to build new facilities should be spent. In this way, the resources that we have could be used where they are most needed. 

## Works Cited 

[1] Armstrong, Corinne E., et al. “Subnational Variation for Care at Birth in Tanzania: Is This Explained by Place, People, Money or Drugs?” BMC Public Health, vol. 16, no. S2, 2016.

[2] Bee, Margaret, et al. “Neonatal Care Practices in Sub-Saharan Africa: a Systematic Review of Quantitative and Qualitative Data.” Journal of Health, Population and Nutrition, vol. 37, no. 1, 2018.

[3] Chojenta, Catherine, et al. “The Impact of Antenatal Care on Neonatal Mortality in Sub-Saharan Africa: A Systematic Review and Meta-Analysis.” PLOS ONE, Public Library of Science.

[4] Deaton, Angus S, and Robert Tortora. “People in Sub-Saharan Africa Rate Their Health and Health Care among the Lowest in the World.” Health Affairs (Project Hope), U.S. National Library of Medicine, Mar. 2015.

[5] Neal, Sarah, et al. “Mapping Adolescent First Births within Three East African Countries Using Data from Demographic and Health Surveys: Exploring Geospatial Methods to Inform Policy.” Reproductive Health, vol. 13, no. 1, 23 Aug. 2016.


