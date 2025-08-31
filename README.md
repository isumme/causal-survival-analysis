# Causal Survival Analysis

**Research Topic:** Exploring Treatment Effect Heterogeneity of Right Heart Catheterization in the SUPPORT Dataset with Time-to-Event Outcomes

**Brief Description:**
I explored the intersection of causal inference and survival analysis to identify subpopulations that are especially harmed or helped by right heart catheterization (RHC) using the SUPPORT dataset. I explored the use of two complementary machine learning models: DeepSurv (for survival prediction) and Causal Survival Forests (for estimating heterogeneous treatment effects). By integrating these models, I found consistent key variables across both survival risk and treatment effect heterogeneity, enhancing the clinical relevance of our findings. This multi-model framework helps to inform more targeted use of RHC in clinical practice.


## ML Models

### Causal Survival Forest
This model was implemented using the causal survival forest model from the grf package. Causal survival forests are used to estimate heterogeneous treatment effects for survival data where the outcomes can be right-censored. It makes splits to maximize treatment effect differences.


### DeepSurv
This model was implemented using the DeepSurv model from the survivalmodels package. DeepSurv is a deep learning generalization of the Cox proportional hazards model. In comparison to causal survival forests, it aims to have strong predictive power.


### Random Survival Forest
This model was implemented using the random survival forest model from the scikit-survival package. Random forests were a later addition to the project. This model ended up outperforming DeepSurv in terms of predictive performance.
