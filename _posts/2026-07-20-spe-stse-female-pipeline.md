---
title: 'Why I Wrote a Paper About Women Dropping Out of Petroleum Engineering'
date: 2026-07-20
permalink: /posts/2026/07/spe-stse-female-pipeline/
tags:
  - research
  - machine learning
  - SPE
  - gender equity
---

SPE STSE 2026 accepted my paper. It's about predicting and preventing female attrition in petroleum engineering pipelines in Africa. I want to explain why I wrote it, because the methodology is public in the paper but the reasoning behind it isn't.

## The question

Nigeria's petroleum sector has some of the worst gender retention numbers in the industry. Women enter petroleum engineering programmes and then leave — either before graduation or early in their careers. The existing research mostly describes the problem. What I wanted to know was whether you could predict it early enough to intervene.

That's a different question. It means: given what we know about a student at the point of first-year enrollment, or about an early-career engineer eighteen months into their first role, can we identify who is at risk before the exit happens?

## The data and the method

I worked with 2,081 records from Nigerian petroleum engineering programmes and industry partners. The dual-stage framing was the structural insight: dropout and career exit are not the same event, they have different predictors, and collapsing them into one model loses information about when and why the attrition happens.

For the student stage I used XGBoost and Random Forest. For the professional stage I added a Neural Network component. SHAP explanations throughout — because a model that tells you someone is at risk but not why is not useful to an administrator or a manager. The top SHAP features at each stage were different, which validated the dual-stage approach.

## What the results showed

The results showed that the predictors at the student stage are dominated by social and environmental factors — department culture, peer group composition, first-year lab experience. Academic performance is less predictive than you'd expect. The machine learning literature on educational attrition often shows this, but it hadn't been applied to this specific pipeline in Nigeria.

At the professional stage the picture shifts: mentorship availability and manager demographics become the strongest predictors.

None of this is surprising in retrospect. But "not surprising in retrospect" is not the same as "known and acted on." Having quantified predictors with SHAP weights is different from intuition.

## Why petroleum engineering specifically

Partly because the SPE Student Technical Symposium and Exhibition is a real venue with a real peer review process. Partly because petroleum engineering is one of the highest-earning engineering tracks in Nigeria, and the gender gap there has large downstream economic effects on women's wealth.

But also: I study computer engineering. Writing a paper about petroleum engineering means I had to learn enough about that world to ask good questions. That constraint was useful. It forced me to be a researcher rather than just a programmer applying a model.

The paper is SPE-STSE-2026-050 if you want to read it.
