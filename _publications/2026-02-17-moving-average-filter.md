---
title: "Design and FPGA Implementation of a 3-Point Moving Average FIR Filter Using VHDL Finite State Machine Architecture on the Altera DE10-Lite Platform"
collection: publications
category: manuscripts
permalink: /publication/2026-02-17-moving-average-filter
excerpt: 'A VHDL FSM implementation of the 3-point moving average FIR filter H(z) = (1/3)(1+z⁻¹+z⁻²) on the Intel MAX 10 FPGA, consuming 47 logic elements and zero DSP blocks, operating at 150 MHz — with functional simulation in ModelSim and hardware verification on the Altera DE10-Lite board.'
date: 2026-02-17
venue: 'EEG 213: Signals and Systems — Department of Electrical and Electronics Engineering, University of Lagos'
paperurl: '/files/moving-average-filter.pdf'
citation: 'Esabu, B. O. (2026). Design and FPGA Implementation of a 3-Point Moving Average FIR Filter Using VHDL Finite State Machine Architecture on the Altera DE10-Lite Platform. EEG 213 Laboratory Report, University of Lagos.'
---

The 3-point moving average filter y[n] = (x[n] + x[n−1] + x[n−2]) / 3 is the simplest non-trivial FIR low-pass filter, with transfer function H(z) = (1/3)(1 + z⁻¹ + z⁻²) and transmission nulls at z = e^(±j2π/3), placing a frequency null at f_s/3. This paper documents the complete FPGA design flow: mathematical characterisation of the Type I linear-phase FIR (1-sample constant group delay), VHDL finite state machine architecture with a 6-state pipeline (IDLE → SHIFT → LOAD → ADD → DIVIDE → OUTPUT), ModelSim functional simulation on step, ramp, and sinusoidal test vectors, Intel Quartus Prime synthesis on the Altera DE10-Lite (Intel MAX 10 10M50DAF484C7G), and live hardware verification using on-board switches and seven-segment displays. Synthesis results: 47 logic elements, 0 DSP blocks, 150 MHz Fmax (3× headroom over the 50 MHz on-board clock). All simulation test vectors verified exactly in hardware.
