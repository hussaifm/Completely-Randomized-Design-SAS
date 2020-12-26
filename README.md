# Completely Randomized Resign CRD (Overview)
1. Abstract 
2. Introduction
3. Design
4. Results
5. Conclusion
# Abstract 
The trout were placed at random in four different troughs. The fish food added to the troughs contained, respectively, 0, 5, 10, and 15g of sulfamerazine per 100 pounds of fish (coded 1, 2, 3, 4). The measurements of hemoglobin (gram per 100ml) in the blood of brown trout were measured after 35 days. The measurements were made on ten randomly selected fish from each trough. We used one-way effects model to test the effect of the sulfamerazine on the hemoglobin measurements, and we compared the differences between each two groups using pairwise test. Also, we used comparisons to control method to compare each group with a control (group 1). We conclude that sulfamerazin can affect the hemoglobin measurements in the Trout. Also, from pairwise all the groups don’t have different effects between each other except the two comparison groups are different (group 1 and 2), and (group 1 and 3) are different.

# Introduction
The data in the table show the measurements of hemoglobin (gram per 100ml) in the blood of brown trout. The trout were placed at random in four different troughs. The fish food added to the troughs contained, respectively, 0, 5, 10, and 15g of sulfamerazine per 100 pounds of fish (coded 1, 2, 3, 4). The measurements were made on ten randomly selected fish from each trough after 35 days. We want to know if the sulfamerazine can affect the hemoglobin measurements, and if it can affect the hemoglobin measurements, how the sulfamerazine doses 0, 5, 10 and 15 are different from each other.

# Design 
We used completely randomized design to answer the research questions. We used one-way effects model yij=μ +τi
=eij. For each group  r_i = 10 so the design is balanced, and we have 4 groups (1= 0g , 2 = 5g , 3 = 10g , 4 = 15g) so t = 4. In this model, the treatment is sulfamerazine and the response variable is the hemoglobin measurements. To answer the question if sulfamerazine can affect the hemoglobin measurements we test the null hypothesis at significance level 0.05 H_0=\ \tau_1=\tau_2=\tau_3=\tau_4\ vs\ H_1:\ not\ all\ \tau_i\prime s\ are\ 0. We can get F = \frac{MST}{MSE}\  from SAS then reject the null hypothesis if F >  F_{0.05}. 
To answer the second question: how are the 4 groups of sulfamerazine are different, we used two methods: 
	Pairwise comparisons (Tukey’s method) to compare mean responses between any two groups and we calculated the 95% confidence intervals, we will perform six comparisons in this scenario. We test this six null hypothesis and we use the p-value to identify the significant comparisons at significant level 0.05:
H_0:\ \tau_1-\tau_2=0 , vs\ H_1:\ \tau_1-\tau_2\neq0\ \bigmH_0:\ \tau_1-\tau_3=0, vs H_1:\ \tau_1-\tau_3\neq0
H_0:\ \tau_1-\tau_4=0, vs H_1:\ \tau_1-\tau_4\neq0
H_0:\ \tau_2-\tau_3=0, vs H_1:\ \tau_2-\tau_3\neq0
H_0:\tau_2-\tau_4=0, vs H_1:\ \tau_2-\tau_4\neq0
H_0:\ \tau_3-\tau_4=0,\ vs\ H_1:\ \tau_3-\tau_4\neq0
	Comparisons to control (Dunnett’s method) we will compare the mean response between the control group and the 95% confidence intervals we will have three comparisons in this scenario. Our control group is group 1 because this is the group that had received 0 g of sulfamerazine and we want to compare each group with group 1. We used the p-value to identify the significant comparisons at significant level 0.05
H_0:\ \tau_2-\tau_1=0, vs H_1:\ \tau_2-\tau_1\neq0
H_0:\ \tau_3-\tau_1=0, vs H_1:\ \tau_3-\tau_1\neq 0
H_0:\ \tau_4-\tau_1=0, vs H_1:\ \tau_4-\tau_1\neq\ 0




