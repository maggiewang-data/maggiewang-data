# Maggie Wang

I studied economics at NYU, and the most useful thing it taught me was suspicion. When two things move together, the interesting question is usually not *how strongly* but *why*, and whether the answer would hold if someone actually intervened. Most of my work as a data analyst comes back to that question.

## What I've worked on

At **InnovaAI**, I worked on user retention. A churn model could rank users by how likely they were to leave, but it couldn't say what would make them stay, and a prediction isn't a lever. So the onboarding question became an experiment instead of a correlation: we changed the flow for a randomized group and measured the difference. It lifted onboarding by 1.85 percentage points, and the effect was large enough relative to its noise (p = 0.004) that the team could act on it rather than argue about it.

At **DoOne Technologies**, the problem came earlier in the chain. Analysis built on a pipeline that was only right 60% of the time was mostly analysis of the pipeline's mistakes. Fixing the data first brought accuracy to 90%, and it removed half the manual cleanup people had been doing every week to work around it.

At **NYU Economics**, I built the data behind a topic-modeling study of news coverage. The raw corpus was skewed 9:1 toward one group of sources, which meant any "topic" the model found would mostly describe those outlets, not the news. Rebalancing to 6:4 before modeling mattered more than any choice of model afterwards.

At **Barnard College**, I first worked on prediction-market data: mapping networks of trades that inflate volume without changing who holds what, and checking whether market prices behave like honest probabilities. Now I build interactive economics teaching modules in R Shiny. Turning a concept into something a student can push on and watch respond is a good test of whether I understand it myself.

## Projects

**[Where an e-commerce marketplace loses its customers](https://github.com/maggiewang-data/sql-product-analytics)**
Real orders from about 100,000 Brazilian marketplace customers, analyzed entirely in SQL. The first finding came before any metric: the table has one customer ID per *order*, not per person, so counting the obvious column makes every returning buyer look new. Counted correctly, only about 2% of customers genuinely come back. And the clearest controllable driver of bad reviews is a late delivery, a gap that holds up inside every state, not just in the remote ones.

**[Did "active choice" raise organ donor sign-ups?](https://github.com/maggiewang-data/did-causal-inference)**
California changed one rule and 26 states didn't, which makes a natural comparison. The standard regression called the drop significant. But with only one state actually treated, that standard error assumes far more independent evidence than exists. When I compared California against every other state's placebo result instead, its change looked ordinary. I report that version, because it's the one that survives the design.

**[Onboarding A/B test, start to finish](https://github.com/maggiewang-data/product-ds-experimentation)**
This rebuilds the InnovaAI kind of experiment in public, on simulated data, so every decision is visible. The order is the point: decide how large an effect is worth detecting *before* launching, confirm the randomization held *before* reading any result, and only then ask whether the gain came at a cost elsewhere. One guardrail came back too noisy to clear or condemn, so the recommendation is to ship and monitor it, not to pretend it passed.

**[From churn score to retention decision](https://github.com/maggiewang-data/churn-ml-pipeline)**
A churn probability only matters once someone decides what to do with it. A missed churner costs months of revenue and an unnecessary offer costs a discount, so the right cutoff isn't 0.5. I set it where expected profit peaks. Then I packaged the model as a service with tests, because a model nobody can call doesn't change any decisions. After launch, a monitor watches each month's customers. In the month a price rise made the model underestimate churn, ranking accuracy actually went *up*, so only the calibration check caught that the probabilities had fallen behind reality.

## Contact

magwang0117@gmail.com · [LinkedIn](https://www.linkedin.com/in/maggiewang17) · New York, open to remote or relocation
