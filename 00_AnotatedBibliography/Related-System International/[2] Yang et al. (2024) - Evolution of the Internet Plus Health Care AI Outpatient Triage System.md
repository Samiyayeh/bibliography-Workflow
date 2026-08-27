# [2] Yang et al. (2024) — Evolution of the "Internet Plus Health Care" Mode: AI Outpatient Triage System

**Category:** [[Related System International]]

## ACM Citation

Lingrui Yang, Jiali Pang, Song Zuo, Jian Xu, Wei Jin, Feng Zuo, Kui Xue, Zhongzhou Xiao, Xinwei Peng, Jie Xu, Xiaofan Zhang, Ruiyao Chen, Shuqing Luo, Shaoting Zhang, and Xin Sun. 2024. Evolution of the "Internet Plus Health Care" Mode Enabled by Artificial Intelligence: Development and Application of an Outpatient Triage System. *J Med Internet Res* 26, (2024), e51711. [https://doi.org/10.2196/51711](https://doi.org/10.2196/51711)

## Annotated Analysis

**Summary:** Deployed at Xinhua Hospital in Shanghai, this system applies an artificial intelligence model trained on 395,790 patient electronic medical records and 500 clinical dialogue groups to automatically direct outpatient walk-ins to the correct specialized department at registration, covering 79 subspecialty departments with a routing accuracy of 0.8945, reducing erroneous registration cancellations from 3.83% to 3.53%, and completing each triage decision in 10.11 seconds compared to 14.33 seconds by human triage nurses.

**Relevance:** The measured reduction in registration errors and the 4.22-second improvement in per-patient triage processing time confirm that replacing manual, nurse-directed department assignment with an automated intake routing mechanism measurably reduces patient misrouting and service congestion at the point of entry. Specifically, the Xinhua system's demonstration that automated department-matching produces statistically superior results to human triage judgment validates the NCHO HIS kiosk-based check-in module, which maps each patient's declared service need to the appropriate queue station and automatically surfaces the corresponding health record on the attending physician's terminal the moment the queue number is called.


## Source References

- **Methods section:** "We collected 395,790 electronic medical records (EMRs) and 500 medical dialogue groups. The triage system was altered based on the current BERT (Bidirectional Encoder Representations from Transformers) framework."
- **Results section:** "Our triage system could accurately recommend 79 subspecialty departments and reduce the number of registration cancellations from 16,037 (3.83%) of the total 418,714 to 15,338 (3.53%) of the total 434,200 (P<.05)."
- **Results section:** "Our triage system significantly outperformed triage nurses in recall@3 (0.6230 vs 0.5266; P<.001) and time consumption (10.11 vs 14.33 seconds; P<.001)."
- **Conclusions section:** "The triage system demonstrates high accuracy in outpatient triage of all departments and excels in subspecialty department recommendations, which could decrease the cancellation rate and time consumption."
