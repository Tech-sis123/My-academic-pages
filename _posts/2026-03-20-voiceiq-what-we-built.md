---
title: 'VoiceIQ: What We Built, and Why Nigerian English Needed It'
date: 2026-03-20
permalink: /posts/2026/03/voiceiq/
tags:
  - machine learning
  - NLP
  - hackathon
  - Nigeria
---

In March we entered the Microsoft AI Skills Hackathon and walked out with first place. This is what we built and why it mattered enough to us to build it seriously rather than just quickly.

## The problem

Nigerian call centres are one of the largest employers of fresh graduates in Lagos. The operators — MTN, Airtel, Glo — run hundreds of agents simultaneously, handling complaints, churn prevention, upselling. The problem is that the NLP tooling those companies use (or could buy) is almost entirely optimised for American or British English.

That sounds like a minor inconvenience. It is not. A subscriber from Kano does not say "I want to cancel." They might say "I don't want this again" in Pidgin, switch to Hausa to explain why, then say "make I just comot the plan." An English-only model scores that as neutral or incoherent. The agent gets no signal. The churn happens.

## What VoiceIQ does

VoiceIQ is a real-time telecom conversation intelligence layer for Nigerian English and Pidgin. Three core components:

**1. Code-switching NLP.** The model identifies language at the utterance level — not the document level — because within a single sentence a caller might blend English, Pidgin, and a local language. We built a language identification layer first, then applied sentiment analysis on top of it per-language segment.

**2. Churn prediction.** We trained an XGBoost model on telco subscriber behaviour features and used SHAP for explainability — so when the model flags high churn risk mid-call, the agent sees not just a score but the top three drivers. "This caller has called billing three times in seven days and has a contract expiry in 30 days." That's actionable. A raw number is not.

**3. Agent Action Cards.** The part I found most interesting to design. These are real-time prompts that surface to the agent as the call progresses — retention offer suggestions, escalation triggers, next-best-action recommendations. The constraint was latency: these have to appear before the caller notices the silence. We used a lightweight inference pipeline to keep the round-trip fast.

## What I learned

I led the idea and the pitch. My teammates Akeem and Yusuf were both sharp and willing to push back on ideas that sounded good but fell apart on second thought — which is the right kind of collaborator for a 48-hour build.

The pitch itself taught me something I knew intellectually but hadn't felt: the gap between understanding a problem and making other people care about it in four minutes is enormous. The judges at a Microsoft hackathon have seen many demo days. What they respond to is specificity. Not "we improve call centre performance" but "here is the exact sentence a caller says that a current model misclassifies, and here is what ours does instead."

We won. We should build the real thing.
