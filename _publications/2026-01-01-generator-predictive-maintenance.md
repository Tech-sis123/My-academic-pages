---
title: "Predictive Maintenance System for Residential Generators Using Acoustic Signal Analysis and Remaining Useful Life Estimation: A Python-Based DSP Approach for Smart Home Applications"
collection: publications
category: manuscripts
permalink: /publication/2026-01-01-generator-predictive-maintenance
excerpt: 'A Python-based DSP framework that captures generator acoustic signals, extracts 9 time- and frequency-domain features via FFT, and predicts remaining useful life using linear regression — validated on real MIMII industrial recordings and deployed as a multilingual web app (English, Igbo, Yoruba, Hausa).'
date: 2026-01-01
venue: 'EEG 213: Signals and Systems — Department of Electrical and Electronics Engineering, University of Lagos'
paperurl: 'https://gendoc.streamlit.app/'
citation: 'Esabu, B. O. (2026). Predictive Maintenance System for Residential Generators Using Acoustic Signal Analysis and Remaining Useful Life Estimation: A Python-Based DSP Approach for Smart Home Applications. EEG 213 Research Paper, University of Lagos.'
---

Residential generators are critical infrastructure for Nigerian households, yet failures are typically detected only after they occur. This paper presents a proactive acoustic monitoring system that extracts nine signal features (spectral centroid, ZCR, RMS energy, dominant frequency, spectral rolloff, spectral bandwidth, and MFCCs 1–3) from generator sound using a 1024-point FFT pipeline with Hamming windowing. A composite health score drives a linear regression model for remaining useful life (RUL) prediction, complete with 95% confidence intervals. The system was validated on the MIMII industrial machine sound dataset, achieving 87.5% classification accuracy and R² = 0.94 on a simulated degradation timeline. A full-stack web application (React + Flask + SQLite) delivers results in English, Igbo, Yoruba, and Hausa, processing each 1-second window in 47 ms — 21× faster than real time. A roadmap for future ESP32 embedded deployment is provided.

**Live app:** [gendoc.streamlit.app](https://gendoc.streamlit.app/) | **Code:** [github.com/Tech-sis123/GenDoc](https://github.com/Tech-sis123/GenDoc)
