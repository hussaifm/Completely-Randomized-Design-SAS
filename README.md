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

![trout table](https://user-images.githubusercontent.com/56862845/103164810-d1e93c00-47dd-11eb-9167-01e33e92f3ab.JPG)


# Design 
We used completely randomized design to answer the research questions. We used one-way effects model yij=μ +τi
=eij. For each group  ri = 10 so the design is balanced, and we have 4 groups (1= 0g , 2 = 5g , 3 = 10g , 4 = 15g) so t = 4. In this model, the treatment is sulfamerazine and the response variable is the hemoglobin measurements. To answer the question if sulfamerazine can affect the hemoglobin measurements we test the null hypothesis at significance level 0.05 H0= τ1 = τ2 = τ3 = τ4 vs H1:not all τi's are 0. We can get F = MST/MSE from SAS then reject the null hypothesis if F > F0.05

To answer the second question: how are the 4 groups of sulfamerazine are different, we used two methods: 

Pairwise comparisons (Tukey’s method) to compare mean responses between any two groups and we calculated the 95% confidence intervals, we will perform six comparisons in this scenario. We test this six null hypothesis and we use the p-value to identify the significant comparisons at significant level 0.05:

H0= τ1 - τ2 = 0 
H0= τ1 - τ3 = 0 
H0= τ1 - τ4 = 0
H0= τ2 - τ3 = 0 
H0= τ2 - τ4 = 0
H0= τ3 - τ4 = 0

Comparisons to control (Dunnett’s method) we will compare the mean response between the control group and the 95% confidence intervals we will have three comparisons in this scenario. Our control group is group 1 because this is the group that had received 0 g of sulfamerazine and we want to compare each group with group 1. We used the p-value to identify the significant comparisons at significant level 0.05

H0= τ2 - τ1 = 0 
H0= τ3 - τ1 = 0 
H0= τ1 - τ4 = 0

# Results
We used SAS software 9.4 to conduct One-Way ANOVA. We tested first null hypothesis H0= τ1 = τ2 = τ3 = τ4 vs H1:not all τi's are 0.\ The P-value in the Type III S table is 0.0027. We reject the null hypothesis at significance level 0.05. In other words, F =MST/MSE = 5.70 and F0.05 (3,36) = 2.86. So, F >  F0.05 The SAS outputs are below:

![SAS affect](https://user-images.githubusercontent.com/56862845/103164370-8bdda980-47d8-11eb-859a-3863179a121b.PNG)
We tested these 6 null hypotheses to compare the means between each two groups using Tukey’s method:
H0= τ1 = τ2 The p-value is 0.0029. We reject the H_0 at significance level 0.05

H0= τ1 - τ3 The p-value is 0.0122. We reject the H0 at significance level 0.05

H0= τ1 - τ4 The p-value is 0.0539. We fail to reject the H0 at significance level 0.05

H0= τ2 - τ3 The p-value is 0.9498. We fail to reject the H0 at significance level 0.05 

H0= τ2 - τ4 The p-value is 0.6660. We fail to reject the H0 at significance level 0.05

H0= τ3 - τ4 The p-value is 0.9292. We fail to reject the H0 at significance level 0.05 
![SAS tukey](https://user-images.githubusercontent.com/56862845/103164546-e6780500-47da-11eb-97b7-10f4bffa0cc2.PNG)
![SAS tukey2](https://user-images.githubusercontent.com/56862845/103164592-7158ff80-47db-11eb-9fd9-f511e56c4699.PNG)

The graph shows the two comparison groups  τ1 - τ2 ≠0 and τ1 - τ3 ≠ 0 only are significant.

![tukey_graph](https://user-images.githubusercontent.com/56862845/103164696-808c7d00-47dc-11eb-91a3-5e9b18bd5ae9.PNG)

We tested the three null hypotheses to compare the control group with other groups using Dunnett’s method and the results:

H0= τ2 - τ1 = 0 The p-value is 0.0015. We reject the H_0 at significance level 0.05

H0= τ3 - τ1 = 0 The p-value is 0.0066. We reject the H_0 at significance level 0.05

H0= τ4 - τ1 = 0 The p-value is 0.0308. We reject the H_0 at significance level 0.05

![dunnetts1](https://user-images.githubusercontent.com/56862845/103164769-59827b00-47dd-11eb-904a-e622bf0277c1.PNG)

# Conclusion 
From One-Way ANOVA test results, we conclude that the sulfamerazine treatment can affect the hemoglobin measurement in the Trout because the p-value is significant. Also, from the pairwise comparisons, we found the group1 who received 0 g sulfamerazine & group 2 who received 5 g are different from each other. Similarly, group1 & group 3 who received 10 g are different from each other unlike the other comparison groups which are not different from each other. Furthermore, we wanted to compare the means of each group using the group that received 0 g of sulfamerazine as a control group. The group 2 which received 5 g is different from the control, and the hemoglobin mean of group 2 is 9.33, the mean difference between group 2 & control is 2.13. The group 3 which received 10 g is different from the control too, and the hemoglobin mean for group 3 is 9.03, the mean difference between group 3 and the control is 1.83. The group 4 which received 15 g is different from the control and the hemoglobin mean of group 4 is 8.69, the mean difference between group 4 and control is the least between all the groups 1.49. So, that means as we increase the treatment doses, the hemoglobin measurements decreases and gets closer to the control.

# Refrences 
Dean,A.P.(2017).Design and Analysis of Experiemnts.Springer













