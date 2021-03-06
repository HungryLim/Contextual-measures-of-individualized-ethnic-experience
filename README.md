# Contextual measures of individual experience (racial and ethnic context)


# Introduction
Can the people, places, and institutions that individuals encounter in their daily lives shape users’ attitudes and behaviors? To examine individual's contextual experience, what measurement should we use? We need to start to find the answer of this question with theories of contextual effect. In other words, we need to consider the mechanism of contextual effect. Some scholars argues that the influx other races or outgroup increases racial threat and it affects people's negative attitudes (Giles and Buckner 1993; Key 1949). On the contrary, other scholars state that inter group interaction reduce stereotype and negative attitude towards outgroup (Oliver and Wong 2003; Welch et al. 2001; Cho and Baer 2011). These two different theories share a crucial point in that contact with other race or outgroup is the key to the mechanism. Therefore, when we consider the context and contact, we should consider how our daily lives and actual experience in micro level environment can be captured by our measurement. Then, with the individualized fine-grained contextual data, we can explore the contextual effect more accurately and more realistically. 

Therefore, in this paper, we used Milieu data which is based on people's actual GPS tracking record and Census block data to test the effect of context on racial resentment. We find that our measure of geographic context does not hold conventional level of statistical significance on racial resentment. We also test the same model with different measures of context (State, county and Census track), but the contextual effect is statistically unreliable. 

However, an interesting finding with the dynamic Milieu measure is that there is systematic mismeasurement of context among non-white respondents. The contextual measure of non-white are systematically distant from the contextual measure of white in terms of racial composition of Census block. It implies that the findings of contextual effect could not be well applied to racial minorities and the systematic mismeasurement could result bias in findings. Using an individual's Census tract as a proxy for social context performs better than the county and state measures. However, here too we see that this measure can under- or over-estimate the percentage of non-white people that an individual encounters. Indeed, Census tracts with a non-white population of around 30% align with dynamic block measures that put the non-white share of the population at nearly 60%.

# Project goals
1) Does individualized racial and ethnic experience (using dynamic measures of racial context) explain individuals' attitudes?
2) Develop new measures of raicial diverity exerience (e.g. using Herfindahl index(HHI)) and compare the measure with conventional static measure.

# Data
In order to create a dynamic measure of racial and ethnic context based on individual milieus, we rely on location data collected for over 400 users of a smartphone application, which automatically records users’ latitude and longitude based on Global Positioning System (GPS) hardware embedded in their mobile phones. Specifically, we obtain a sample of users of the OpenPaths application, developed and maintained by the Research and Development Lab at the New York Times Company. Our sample of OpenPaths users includes 2.6 million data points from 446 individuals. The number of GPS points for each individual range from 1 to over 111,000 with the median number of coordinate pairs being about 3,200. On average, we have about a year’s worth of geolocation for the individuals (364.4 days) with a maximum of over four years’ worth of data. The detailed information about the Milieu data can be found from [here](http://www.andrewreeves.org/papers/context.pdf).

<p align="center">
<img src="graphs/millieu1.PNG" width="300" //>
<img src="graphs/dash.PNG" width="300" //>
<img src="graphs/question.PNG" width="300" //>
</p>


 # Dependent variables
* Direct measure for racial attitudes: Racial Resentment, Views on the Confederate Flag, Views on Immigration Levels, Views on Whether People Can Be Trusted

* Inirect measure for racial attitudes: Whether New Prisons Should be Built, Views on buidling basketball

 # Independent variables
* Pct. Non-White (Dynamic measure)
* Pct. Non-White (Census Tract measure)
* Pct. Non-White (County measure)
* Pct. Non-White (State measure)
* Diversity measure (HHI measure)


# Racial experience measure: Pct. Non-White (Dynamic measure)
The below plot shows the distribution of their racial experience (Census tract-level non-white population based on GPS coordinates from cell phone application). Unlike static measure based on Zipcode or street address, dynamic measures contrain ample information about user's contextual racial experience. The red line in the plot is the degree of percent non-white based on Zipcode of a user. On the other hand, the density plot shows that how each individuals have stayed in different places and have more diverse racial experience. The two measures (dynamic and static) are surprisingly different. 

<p align="center">
<img src="graphs/Dynamic.png" width="600" //>
</p>


# Measurement for racial diversity (or racial sergregation)
<p align="center">
 <a href="https://www.codecogs.com/eqnedit.php?latex=HHI=\sum_{i=1}^{\text{Number&space;of&space;groups}}&space;{\text{Size&space;of&space;a&space;group&space;as&space;a&space;percent&space;of&space;population}_i&space;}^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?HHI=\sum_{i=1}^{\text{Number&space;of&space;groups}}&space;{\text{Size&space;of&space;a&space;group&space;as&space;a&space;percent&space;of&space;population}_i&space;}^2" title="HHI=\sum_{i=1}^{\text{Number of groups}} {\text{Size of a group as a percent of population}_i }^2" /></a>
 </p>

HHI can be maximized if individuals are evenly distributed among R groups. The higher HHI, the more diverse an area is. HHI varies from 0, where all neighborhoods have same composition as the entire city, to 1, where all neighbors have only one group. HHI can be interpreted as a diversity measure and a segregation measure (1 - HHI = segregation measure). 


The below plot shows that how racial diversity (i.e. segregation measure). Rather than using the percent non-white of census track, I generated a new measure of segregation measure. This measure can be useful where a researcher wants to know not just non-white experience, but the degree of experience from racial diversity or segregation. Again the red line is a user's measure for degree of racial segregation based on Zipcode. In this time, the dotted line is the measure for the weighted and aggregated experience of racial segregation.

<p align="center">
<img src="graphs/HHI.png" width="600" //>
</p>

# Method


# Results

<p align="center">
<img src="graphs/recent_t.PNG" width="600" //>
</p>


<p align="center">
<img src="graphs/hhi_t.PNG" width="600" //>
</p>

<p align="center">
<img src="graphs/Rplot03.png" width="800" //>
</p>

while the plots in Figure 2 are informative of a mismatch between the contexts cap-
tured by our dynamic measure and those captured by static measures, they do nothing to indicate
the degree of these mismatches nor the specific factors that are predictive of such mismatches.
To better understand the degree to which our dynamic measure captures a different context than
these commonly used static measures, we separately calculated the absolute difference between
the percentage of non-white individuals in the context measured by our dynamic measure and the
percentage of non-white individuals measured by the contexts captured by an individual's state,
county, and Census tract of residence. The mean difference between our dynamic measure and an
individual's state of residence is 12.43; the mean difference between our dynamic measure and one's
county of residence is 10.31; finally, the difference between our dynamic measure and an individual's
Census tract of residence is 7.1. This suggests that, in terms of accurately capturing the context
that an individual experiences throughout his or her daily life, Census tract measures perform the
best, county measures perform second best, and state measures perform the worst.

<p align="center">
<img src="graphs/mismeasure.png" width="800" //>
</p>


To determine the factors most associated with these mismatches, we regressed each of the difference measures described above on a series of political and sociodemographic characteristics. These measures include dummy variables for Democrats and Republicans, as well as measures of race, gender, age, educational attainment, and income. The results of these regressions are presented in Table \ref{tab:differences}. Most notable are the positive coefficients on our non-white dummy variable. This indicates that using either the state or county of residence as a proxy for social context is likely to yield larger mismeasurements of the percentage of non-white individuals that one sees for those individuals who \emph{are} non-white compared to those who are white. A similar relationship exists when comparing our dynamic measure of social context to one's Census tract of residence, though this relationship is not statistically significant at conventional levels. Models run measuring the real distance between our dynamic measure of social context and these static proxies suggest that using an individual's state of residence as a proxy underestimates the percentage of non-white people that non-white individuals see by $14\%$. Using the county of residence as a proxy underestimates the percentage of non-whites that non-white individuals encounter by nearly $10\%$.\footnote{These models can be found in Table \ref{tab:directional} in the Appendix.}

In addition to these racial differences in mismeasurement, the results of Table \ref{tab:differences} indicate that a few other covariates are associated with measurement error. Interestingly, education levels are associated with better (column one) and worse (column three) measurements of the percentage of non-white individuals that one encounters. Additionally, using an individual's Census tract of residence tends to mismeasure the percentage of non-white individuals that Democrats encounter.

<p align="center">
<img src="graphs/diff_measure_t.PNG" width="400" //>
</p>

This project is collaborated with [Andrew Reeves](http://www.andrewreeves.org/), [Steven Webster](http://www.stevenwwebster.com/), and [Ryan Moore](http://www.ryantmoore.org/).
