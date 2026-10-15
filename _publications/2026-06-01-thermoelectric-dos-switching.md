---
title: "Adaptive Density-of-States Switching for Performance Optimization in Thermoelectric Energy-Harvesting Systems: A C++ and MATLAB Computational Framework"
collection: publications
category: manuscripts
permalink: /publication/2026-06-01-thermoelectric-dos-switching
excerpt: 'A validated C++/MATLAB computational framework showing that adaptive switching between DOS-engineered thermoelectric elements outperforms any fixed single element by 1.3–2.0% under volatile operating profiles, with a 5% advantage over the average fixed choice — and that a cost-aware controller is essential to preserve the gain.'
date: 2026-06-01
venue: 'EEG 226: Physical Electronics — Department of Electrical and Electronics Engineering, University of Lagos'
paperurl: ''
citation: 'Esabu, B. O. (2026). Adaptive Density-of-States Switching for Performance Optimization in Thermoelectric Energy-Harvesting Systems: A C++ and MATLAB Computational Framework. EEG 226 Research Paper, University of Lagos.'
---

Thermoelectric generators convert heat to electricity, but a fixed material is efficient only within a narrow temperature window. This work investigates whether a bank of thermoelectric elements — each DOS-engineered via a Lorentzian resonant peak for a different temperature range — can harvest more energy than any single fixed element by dynamically switching between them. A transport physics framework was implemented in C++ (primary numerical core under the constant relaxation-time approximation) and independently re-implemented in MATLAB for cross-validation; both cores agree to five significant figures across all test points. Results across temperature profiles of varying volatility show a consistent adaptive gain of 1.3–2.0% over the best fixed element, rising with profile volatility, and approximately 5% over the average fixed choice. The most practically significant finding is robustness: because the optimal fixed element changes with the operating profile, adaptive control removes the need for foreknowledge. A naive controller loses its advantage entirely at high switching costs; a hysteresis-based cost-aware controller preserves a net positive gain at all tested cost levels.
