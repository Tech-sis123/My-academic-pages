---
title: 'EthnoLedger: Why We Built a Blockchain System for Indigenous Knowledge with a Keypad'
date: 2026-08-15
permalink: /posts/2026/08/ethnoledger/
tags:
  - blockchain
  - DeSci
  - Nigeria
  - indigenous knowledge
---

EthnoLedger was published at DeSci Lagos in August. The core idea: USSD-blockchain for indigenous knowledge preservation. I want to explain why USSD matters, because people outside Nigeria usually ask why we didn't just build an app.

## The problem with apps

Smartphone penetration in Nigeria is real and growing. But "growing" means uneven. A subsistence farmer in Benue State who holds twenty years of knowledge about drought-resistant yam cultivar management does not necessarily have a smartphone. They almost certainly have a basic phone. That phone has USSD.

USSD is the protocol that runs on every phone with a SIM card — no data plan, no internet, no app. You dial a string like *737# and a session begins. It's how millions of Nigerians access banking, government services, airtime purchases. It's one of the most robust and widely deployed interaction paradigms in sub-Saharan Africa, and the tech industry almost entirely ignores it.

The knowledge we are losing — agricultural practices, herbal medicine, oral historical records, ecological observations — is concentrated in communities where USSD is the realistic interface.

## What EthnoLedger actually is

A knowledge holder dials a USSD code, navigates a structured session to contribute a piece of knowledge, and that contribution is hashed, timestamped, and recorded on-chain. The blockchain layer exists for two reasons: tamper-evidence (the record of a contribution can't be retroactively altered) and provenance (if this knowledge becomes commercially valuable, the originating community has a cryptographic record of precedence).

The USSD layer handles the input. The chain handles the permanence and the attribution. We built a bridge service that translates USSD session data into chain transactions without requiring the contributor to know anything about blockchain infrastructure.

## What we presented at DeSci Lagos

DeSci Lagos is a decentralised science event focused on applying Web3 infrastructure to African challenges — open data, research provenance, public-good science funding. It's a community that takes seriously the question of what "open science" means in a context where most scientific publishing infrastructure was built for and by institutions in the Global North.

We presented EthnoLedger as both a technical system and an argument: that preservation infrastructure for indigenous knowledge needs to be designed around the access constraints of the people whose knowledge it is. Building a platform that works on desktops for researchers to document communities is not the same thing as building a platform the communities themselves can use.

## What comes next

The hard part is not the architecture. The hard part is community onboarding: convincing knowledge holders that contributing to this system is safe, that their intellectual property is protected, that the system serves them and not a researcher extracting data. That's a trust problem and a governance problem, not a technical one.

I don't have a clean answer to it yet. But I think it's the right question to be working on.
