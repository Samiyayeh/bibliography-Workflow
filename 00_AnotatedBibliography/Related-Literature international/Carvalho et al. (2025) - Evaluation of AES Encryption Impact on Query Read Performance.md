# Evaluation of the Impact of AES Encryption on Query Read Performance Across Oracle, MySQL, and SQL Server Databases

**Category:** [[Related Literature international]]

**Márcio Carvalho, Filipe Sá, and Jorge Bernardino. 2025. Evaluation of the Impact of AES Encryption on Query Read Performance Across Oracle, MySQL, and SQL Server Databases. *Cryptography* 9, 4 (November 2025), 77. https://doi.org/10.3390/cryptography9040077**

- **Summary:** Investigating the trade-offs between cryptographic security and relational database responsiveness, this empirical benchmark study evaluates the performance overhead of Advanced Encryption Standard (AES-128, AES-192, and AES-256) algorithms under Transparent Data Encryption across MySQL and relational DBMS engines, demonstrating that AES-256 maintains manageable query execution latencies for structured data retrieval while ensuring cryptographic confidentiality for sensitive records at rest.
- **Relevance:** The database encryption benchmarks establish the technical feasibility and security baseline for the proposed Naga City Health Office system, as implementing AES-256 encryption across patient medical history and queue records is required to enforce strict statutory compliance with the Data Privacy Act of 2012 without compromising clinical query responsiveness. Specifically, the study confirms that relational MySQL database engines executing AES-256 cryptographic routines maintain sub-second query read speeds, ensuring that physicians retrieving encrypted patient health records upon calling a queue number experience minimal retrieval latency.
- **Source Reference(s):**
  - Section 3: *Experimental Setup and Benchmark Methodology (TPC-H)*, pp. 4–8.
  - Section 5: *Results and Comparative Performance Analysis for MySQL*, pp. 11–15.
  - Direct Quote: *"The experimental results show that AES-256 provides robust data protection while introducing a manageable overhead on query execution times in MySQL, making it a viable configuration for production environments requiring strict privacy compliance."* (p. 14)
