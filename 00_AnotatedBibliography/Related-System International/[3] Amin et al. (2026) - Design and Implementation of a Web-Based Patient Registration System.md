# [4] Amin et al. (2026) — Design and Implementation of a Web-Based Patient Registration System in a Single-Centered Tertiary Care Hospital of Coastal Karnataka

**Category:** [[Related System International]]

## ACM Citation

Ashwitha N. Amin, G. Somu, Prajwal L. Salins, and Roshan David Jathanna. 2026. Design and Implementation of a Web-Based Patient Registration System in a Single-Centered Tertiary Care Hospital of Coastal Karnataka. *BMC Health Services Research* 26, 1 (2026). https://doi.org/10.1186/s12913-026-14299-3

## Annotated Analysis

**Summary:** Conducted in two phases at Kasturba Hospital in Udupi, India, this prospective observational study first documented that paper-based outpatient registration consumed an average of 17 minutes and 25 seconds per patient — with 25.5% of surveyed patients complaining specifically about waiting lines — then developed a web-based registration platform using the Django framework and MySQL database, integrated into the existing hospital system via a browser plugin for pilot testing, finding that 90.5% of patients were ready to adopt digital registration and 83% believed it would reduce their wait time.

**Relevance:** The documented 17-minute paper-based registration delay and the 90.5% patient readiness for digital intake directly validate the operational problem that the proposed Naga City Health Office system is designed to resolve, as both institutions share the same root cause — manual, paper-driven registration creating a queue bottleneck before any clinical service is reached. Specifically, the study's two-phase approach of first measuring existing paper-based delays before designing a targeted digital replacement mirrors the NCHO HIS development rationale, where observed registration congestion and fragmented physical logbooks motivated the system's centralized digital intake module. In contrast to Kasturba Hospital's standalone browser-plugin-based registration layer, the NCHO HIS integrates the patient registration step directly into the queue assignment process, so that completing check-in simultaneously places the patient in the appropriate service queue and makes their health record immediately accessible to the attending physician — eliminating the gap between registration completion and clinical readiness.

## Source References

- **Results section:** "The time it took to register patients averaged 17 min and 25 s in total, and it took 6 min and 2 s on average for the staff to serve the patients."
- **Results section:** "25.5% voiced their complaints mainly because of the long waiting lines."
- **Results section:** "90.5% of them were ready to utilize such a system if it was introduced. Moreover, 83% of the respondents thought that the online registration system would allow them to spend less time waiting."
- **Methods section:** "The Django framework was used to develop the system with MySQL as the backend database. To ensure the smooth integration with the existing hospital system, a special browser plugin was created."
- **Conclusions section:** "The system for online registrations developed as part of this study is both technically viable and appreciated by the patients."
