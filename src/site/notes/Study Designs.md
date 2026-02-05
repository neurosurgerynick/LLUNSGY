---
{"dg-publish":true,"permalink":"/study-designs/","created":"2024-05-14T08:19:46.000-07:00","updated":"2026-02-04T20:51:33.860-08:00"}
---


![Pasted image 20240521174935.png](/img/user/assets/Pasted%20image%2020240521174935.png)
![[Pasted image 20240514081952.png \| 600]]
# Cohort vs. Case-control studies
## Cohort Studies
**Retrospective cohort** is looking at disease **Incidence** just like all cohort studies
	The groups compared differ by a risk factor at the beginning and are looked at for the incidence of disease between exposed individuals and non exposed individuals
Relative risk is an appropriate measure to analyze
#### Relative Risk: calculated at the end of the analysis for cohort studies
The risk of people exposed developing the disease / the risk of non-exposed individuals developing the disease
```
Risk exposed / Risk non-exposed
```
![Pasted image 20240521141733.png](/img/user/assets/Pasted%20image%2020240521141733.png)
#### Hazard Ratio: calculated instantaneously at different points in the analysis
These studies compare incidence meaning that you calculate a hazard ratio = instantaneous event rate = time to event analysis = survival analysis for total survival time 
		Note that relative risk is not technically the same as a hazard ratio
		Relative risk tells you the risk that someone will have an outcome in the treatment arm vs. the control arm by the end of the analysis
			RR = 1.36 means that the incidence of developing a disease for an exposed person is 36% compared to someone who is not exposed
			RR = 3.36 means that the incidence of developing a disease for an exposed person is 226% compared to someone who is not exposed
		In contrast, [[Hazard ratio\|Hazard ratio]] is an instantaneous measure, and is calculated as time goes on
	or a median survival time for the median

## Case-control studies
**Case-control** studies control for the cases, and compare the **risk factor frequency** between the groups.
Because case-control studies vastly underrepresent the # of people in the population without the disease of interest, you **cannot calculate any risks**
	E.g. a sample of 100 people with tennis elbow and compare them against 100 people without tennis elbow
	To determine the actual risk of developing tennis elbow for single-handed players, you need to take the # of people who developed tennis elbow in single-handed play / the total number of single handed players
	This is impossible in a case-control study because you have no idea how many total single-handed players there are. 
Instead, you can calculate an **Odds Ratio** which can approximate the relative risk if the incidence of the disease is low
	this is called the "rare disease assumption"
![Pasted image 20240521141346.png](/img/user/assets/Pasted%20image%2020240521141346.png)
![Pasted image 20260204195125.png](/img/user/assets/Pasted%20image%2020260204195125.png)
In this example, OR of developing aflatoxin poisoning with indoor storage is:
32/20 divided by 8/80 = 1.6 / 0.1 = 16.0
Mathematically, you can also get there by:
32x80 divided by 20x8 = 16.0

![Pasted image 20240521141709.png](/img/user/assets/Pasted%20image%2020240521141709.png)

The outcomes are controlled for, thus a case control study is only able to assess a single outcomes between the groups
however, it is able to assess for multiple risk factors at the same time
	ie all cases of MDR tuberculosis admitted to hospital
	Separate into risk factors like HIV status, previous treatments, major co-morbidities
### Odds Ratio confidence intervals
The odds ratio is positively skewed, meaning the odds can go from 1 (no difference) until infinity 
To calculate a confidence interval therefore, you need to use the log (OR) which is approximately normally distributed

eg. OR = 2.37
ln(OR) = ln (2.37) = 0.8

Standard Error for the ln(OR)
= sqrt ( 1/A + 1/B + 1/C + 1/D) = 0.306

95% confidence interval, you must use the appropriate z score = 1.96 for a 2 tailed distribution
95%CI ln(OR) = 0.8 +/- 1.96 x 0.306
0.257 < lnOR < 1.458

To get everything out of the log format, we use the base e and revere the natural log
95% CI (OR) = e^.257 < OR < e^1.458
1.293 < OR < 4.298