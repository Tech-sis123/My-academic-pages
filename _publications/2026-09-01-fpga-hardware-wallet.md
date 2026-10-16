---
title: "Design and Implementation of a Side-Channel Resistant FPGA-Based Signing Engine For Cryptocurrency Hardware Wallets"
collection: publications
category: manuscripts
permalink: /publication/2026-09-01-fpga-hardware-wallet
excerpt: 'An FPGA-based signing engine for cryptocurrency hardware wallets, implementing secp256k1 ECDSA with side-channel resistance through Montgomery ladder scalar multiplication — synthesised on the MicroPhase A7-Lite in Vivado and demonstrated on a public testnet.'
date: 2026-09-01
venue: 'Department of Computer Engineering, University of Lagos'
paperurl: '/files/available-upon-request.pdf'
citation: 'Anointein, O. M., & Esabu, B. O. (2026). Design and Implementation of a Side-Channel Resistant FPGA-Based Signing Engine For Cryptocurrency Hardware Wallets. University of Lagos.'
---

This paper presents the design and implementation of a side-channel resistant signing engine for cryptocurrency hardware wallets, targeting the MicroPhase A7-Lite FPGA. The core cryptographic primitive is secp256k1 Elliptic Curve Digital Signature Algorithm (ECDSA), the signature scheme underlying Bitcoin and most EVM-compatible blockchains. Scalar multiplication — the computationally dominant and security-critical operation in ECDSA — is implemented using the Montgomery ladder algorithm, which executes a constant-time, constant-sequence set of field operations regardless of secret key bit values, providing resistance to simple power analysis (SPA) and timing side-channel attacks. The implementation includes a Python reference model for algorithm-level validation and VHDL bring-up files for the FPGA target, synthesised and verified in Vivado. The final prototype operates as a fully standalone device and successfully executes complete transaction signing on a public testnet.

*Co-authored with Obiyor Mitchell Anointein.*
