---
title: "Open-Source SCADA for National Grid Reliability: A Cost-Effective Supervisory Control Framework for Nigeria's Power Infrastructure"
collection: publications
category: manuscripts
permalink: /publication/2026-08-01-scada-power-grid
excerpt: 'A cost-benefit and technical architecture study proposing an open-source SCADA framework (Rapid SCADA, OpenMUC, OpenPDC) conforming to IEC 61850 and IEEE C37.118 for Nigeria's national grid, projecting 53% capital cost reduction ($85M vs $180M) and SAIDI improvement from 4,500+ hours/year to under 1,200 hours/year.'
date: 2026-08-01
venue: 'Department of Electrical and Electronics Engineering, University of Lagos'
paperurl: '/files/scada-power-grid.pdf'
citation: 'Esabu, B. O. (2026). Open-Source SCADA for National Grid Reliability: A Cost-Effective Supervisory Control Framework for Nigeria''s Power Infrastructure. Department of Electrical and Electronics Engineering, University of Lagos.'
---

Nigeria's national grid records over 4,500 hours of customer outage per year (SAIDI), costs the economy an estimated $29 billion annually (~10% of GDP), and suffered 12 total system collapses in 2024 alone. Proprietary SCADA systems from established vendors carry a prohibitive capital cost — approximately $180 million for national-scale deployment. This paper proposes a three-tier open-source supervisory control and data acquisition (SCADA) architecture built on Rapid SCADA (HMI/historian), OpenMUC (IEC 61850 field device gateway), and OpenPDC (IEEE C37.118 phasor data concentrator) for wide-area monitoring. The framework is validated against the IEC 61850 communication standard for substation automation and the IEEE C37.118 synchrophasor measurement standard. A topology analysis of Nigeria's 330/132 kV transmission network identifies 38 priority substations whose instrumentation would achieve maximum observability. A comparative cost model demonstrates a 53% capital expenditure reduction ($85M vs $180M) relative to a representative proprietary deployment of equivalent scale, without sacrificing standards compliance. Reliability projections based on international open-source SCADA deployments (Ukraine's Ukrenergo, Kenya Power) indicate SAIDI improvement from 4,500+ to under 1,200 hours per year within a 5-year implementation horizon. Cybersecurity considerations for ICS/OT environments, including network segmentation and IEC 62351 key management, are addressed as a critical design constraint.
