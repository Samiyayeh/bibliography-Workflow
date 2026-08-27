# [8] Zou et al. (2026) — Analysis of the Anti-Scalping Mechanism of Hospital Appointment Registration Based on Bayesian Theory

**Category:** [[Related System International]]

## ACM Citation

Xiangkun Zou, Lei Wang, Jing Sun, Shengyu Guo, and Yunzeng Huang. 2026. Analysis of the anti-scalping mechanism of hospital appointment registration based on Bayesian theory. *Frontiers in Public Health* 14 (2026). https://doi.org/10.3389/fpubh.2026.1724649

## Annotated Analysis

**Summary:** To combat speculative appointment hoarding that was locking legitimate patients out of clinic slots at a high-volume Chinese hospital, this study implemented and retrospectively evaluated a Bayesian behavioral detection algorithm that flagged abnormal booking patterns — such as registrations completed in under 2 seconds or single devices linked to 5+ patient IDs — demonstrating that the mechanism raised appointment completion rates from 64.6% to 78.0%, cut no-show rates from 35.4% to 22.0%, and drove online registration adoption from 65.6% to 94.5% over four years.

**Relevance:** The appointment integrity mechanism validates the patient verification logic of the proposed Naga City Health Office system, as demonstrating that algorithmic validation of registration behaviors prevents queue manipulation and improves legitimate patient access confirms that digital queue entries must be tied to verified patient identities. Specifically, the system's outcome — a 13.4 percentage-point improvement in appointment completion rates — reinforces the NCHO HIS kiosk design, where queue tickets are issued only upon confirmed patient identity matching against a centralized health record, preventing duplicate entries and phantom queue slots.

## Source References

- **Results section:** "The appointment completion rate improved from 64.6% (2019) to 78.0% (2022) and the no-show rate dropped from 35.4% to 22.0% following implementation."
- **Results section:** "Online registration usage rose from 65.6% in 2020 to 94.5% by 2023 as a result of the anti-scalping mechanism increasing trust and accessibility of the digital booking platform."
- **Methods section:** "The Bayesian model flagged abnormal behaviors: more than three cancellations within 48 hours, a single device ID linked to more than five medical card IDs, or registration completion speeds faster than the 99th percentile of manual operation times."
