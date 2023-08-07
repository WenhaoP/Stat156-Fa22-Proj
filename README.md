**Evaluating the Causal Relationship between Economic Growth and Civil Conflict: A Critical Re-appraisal**
[Link](https://drive.google.com/file/d/1ZHcK9jtgeJEtlPmcP4_CmxKcbdn70_Lk/view)

**Introduction**

The intricate relationship between economic fluctuations and civil conflicts has long piqued the interest of economists, sociologists, and political scientists. This interplay holds significant implications for policy development, especially in regions susceptible to political instability. The seminal paper, "Economic Shocks and Civil Conflict: An Instrumental Variable Approach," delved into this complex nexus, suggesting that economic downturns, specifically negative economic shocks, significantly influence the onset of civil conflict. Using an instrumental variable approach, the authors sought to isolate the causal effects of economic alterations on political discord.

As the findings of this paper are pivotal to our understanding of conflict dynamics and economic policies, ensuring the robustness and reliability of its results is paramount. This replication study endeavors to re-examine the methods, datasets, and conclusions presented in the original work. Our objective is twofold: first, to validate the findings and methodologies of the initial research, ensuring their credibility, and second, to explore any potential nuances or alternative interpretations that might add depth to the original study's insights. 

**Contribution**


Our contribution in this paper is threefold. First, we found that the effect of economic conditions on civil conflict is much more variable than the original paper proposed. This is due to the weak instrumental variable used to estimate the causal effect, which results in two-stage least squares estimates having overly narrow confidence intervals. To address this issue,

we re-analyzed the data using the Fieller-Anderson-Rubin (FAR) method, a non-parametric method of constructing confidence intervals that is more robust to weak instruments and relaxes the assumption of asymptotic normality.

Our second contribution is that we not only replicated the statistical analysis in (Miguel et al., 2004), but we also provided detailed code for the data cleaning process. While the original authors provided documentation of their data cleaning steps, they did not share their code. Our replication efforts ensure transparency and reproducibility of the analysis from start to finish, allowing other researchers to build upon our work and improve the quality of
the findings.

Our third contribution is to enhance the accessibility of the authors’ analysis code by translating it from STATA to R, an open-sourced programming language. While the original authors provided code for their statistical analysis, it was written entirely in STATA, which requires a proprietary software license that may limit access, particularly in Sub-Saharan African countries where this research is more relevant and could have a more significant impact on policy and practice. By translating the code into R, we have eliminated the need for a costly license and made the analysis more widely accessible to researchers worldwide.
