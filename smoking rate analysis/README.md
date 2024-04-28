<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#data-source">Data Source</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#result">Result</a>
    </li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
This research project is divided into two distinct but interrelated parts, 
each addressing separate facets of tobacco use across various demographics in the United States.

1) The research question of interest relates to the variation among the US states that exist and that there is a 
variation from one school to the next, A secondary task is to 
convey the differences in the effect of age on smoking for white, Black, and Hispanic Americans. The effect is 
expected to be different by sex and by rurality. Two hypotheses are made as follows:

* Geographic variation (between states) in the rate of students smoking cigarettes is substantially greater
than the variation amongst schools. As a result, tobacco control programs should target the states with the
most smoking and not concern themselves with finding particular schools where smoking is a problem.
* Rural-urban differences are much greater than differences between states.

2) The research question of interest concerns the usage of cigars among white, black, and Hispanic
Americans, and the likelihood of having used an electronic cigarette for two individuals of different
sexes. Two hypotheses are made as follows:

* Smoking of cigars, cigarillos, or little cigars is no more common amongst Americans of European
ancestry than for Hispanic-Americans and African-Americans, once one accounts for the fact that white
Americans are more likely to live in rural areas and cigar smoking is a rural phenomenon.

* The likelihood of having used an electronic cigarette on at least one occasion is the same for two
individuals of different sexes provided their age, ethnicity, and other demographic characteristics are
similar.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Data Source
The dataset used in this study is from 2019 American National Youth Tobacco Survey, which contains
over 18000 surveys from American youth of different races:
<a href="http://pbrown.ca/teaching/appliedstats/data/smoke.RData"> data source </a>

### Built With

![Language](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)  
![Language](https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)  


<!-- RESULT -->
## Result

The first part modeled the relation between each age, gender, race, and urban/rural with the probability of
smoking cigarettes among teenagers within different schools and states. It counts the specific random effect
of school and state, and as a result, the data does not support the hypothesis that geographic variation in
the rate of students smoking cigarettes is substantially greater than variation amongst schools, but also put
forward that variation amongst school has a higher probability of being greater than variation amongst states.
When considering the effect of urban/rural, this research finds out that a person in a rural area is around
(1.609, 15.737) times the odds of smoking cigarettes as a person in an urban area. While a person in
the smoking state with one standard deviation is around (1.145, 1.565) times the odds of smoking
cigarettes as the person in a typical state. Hence the study suggests that Rural-urban differences are greater
than differences between states.  

It is also crucial that the research finds out that age effects on smoking for white and Hispanic Americans
are different by rurality, but not sex. First of all, the effect of age on smoking acts on all three races would
be decreased as they are older (age 17-18). The effect of age on white and Hispanic Americans smoking
cigarettes is low when the age is around 11 -14 in urban areas, on the contrary, the effect is more efficient when they
are ages of 14-18 compared to black Americans. While in rural areas, they have a higher probability
of smoking at a young age and have a smoother increase over age compared to urban areas. Black
Americans, on the other side, seem to have a similar growth of probability of smoking as age growth under
the effect of urban/rural. For different sexes, neither three of them would impact the age effect on smoking.

The second part modeled the relation between each race, gender, and age with the proportion of cigars and e-cigarette usage among youth by using the 2019 American National Youth Tobacco Survey.It revealed that
Smoking of cigars is no longer common in Americans of European ancestry than for Hispanic Americans and
African-Americans. It also revealed that given age, ethnicity, and other demographic characteristics similar,
the probability of males and females you of tried e-cigarettes is very close to each other with a maximal
percentage difference of 5.
