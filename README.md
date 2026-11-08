# Hi, I'm Maggie

I'm a data analyst in New York with an economics degree from NYU, and I can't shake one habit: before I trust a number, I want to know where it came from. So most of my work comes back to the same question: **did this change actually cause the result, or did it just happen at the same time?**

- NYU '26, B.A. Economics, minors in Data Science and French
- Research assistant at **Barnard College**, building interactive economics teaching modules in R Shiny, and at **NYU** (quantitative economic history)
- Languages: English and Mandarin (fluent), French (working)
- magwang0117@gmail.com · [LinkedIn](https://www.linkedin.com/in/maggiewang17)

---

## Things I've built

**[Onboarding A/B test, start to finish](https://github.com/maggiewang-data/product-ds-experimentation)**
I've run an onboarding experiment for real at InnovaAI. This is the full workflow, done in public on simulated data: sizing the test before launch, checking the randomization before reading any result, CUPED, guardrails, and a one-paragraph memo a PM could act on.

**[Churn model → working API](https://github.com/maggiewang-data/churn-ml-pipeline)**
A churn score is only useful if someone acts on it. So instead of stopping at AUC, I chose *who gets a retention offer* by expected dollars, not a default 0.5 cutoff, and shipped the model as a tested FastAPI service in Docker.

**[One state changed a rule. Did it work?](https://github.com/maggiewang-data/did-causal-inference)**
California made drivers actively choose whether to become organ donors. I used difference-in-differences against 26 other states. The regression says "significant." Randomization inference, which is the right tool when only one state is treated, says p = 0.19. I report the second one.

## Before this

- **InnovaAI Tech:** retention analysis on 55K users. Built 4 user segments, a churn model, and an onboarding A/B test that lifted completion **+1.85 pp (p = 0.004)**
- **DoOne Technologies:** fixed a data pipeline from **60% → 90%** accuracy and cut manual processing in half across 5,000+ weekly records
- **NYU Economics:** topic modeling on **1M+ news articles**, after rebalancing a source mix that was skewed 9:1

## How I work

- I check whether the randomization worked *before* I look at the lift.
- I'd rather report an honest p = 0.19 than a flattering p = 0.001.
- I write the decision, not just the notebook.

**Tools:** Python (pandas, scikit-learn, statsmodels, XGBoost) · SQL · R · FastAPI · Docker · Git

*Looking for data analyst, product analyst and data science roles: New York, remote, or anywhere worth moving for.*
