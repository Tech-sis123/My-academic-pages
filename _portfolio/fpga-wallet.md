---
title: "FPGA-Based ECDSA Signing Engine — Side-Channel Resistant Hardware Wallet"
excerpt: "secp256k1 ECDSA signing engine on MicroPhase A7-Lite (Vivado). Montgomery ladder scalar multiplication for side-channel resistance. Demonstrated on a public Ethereum testnet."
collection: portfolio
---

**Published in Department of Computer Engineering, University of Lagos, 2026**  
*Co-authored with O. M. Anointein*

A side-channel resistant hardware signing engine for cryptocurrency wallets, implementing secp256k1 ECDSA — the elliptic curve used by Bitcoin and Ethereum. Synthesised on the MicroPhase A7-Lite FPGA in Vivado.

**Security approach:** Montgomery ladder scalar multiplication makes the computation time-constant with respect to the private scalar, eliminating the timing and power variations that simple double-and-add implementations leak to an attacker.

**Validation:** Demonstrated signing and verification on a public Ethereum testnet with on-chip key storage and no software fallback.

Hardware security research at the undergraduate level is uncommon in Nigerian Computer Engineering departments. This project was an attempt to change what "computer engineering coursework" can look like.

[Read the paper →](/publications/)
