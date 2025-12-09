Th️ Threat Hunting Notebooks
Analysis, detection and investigation in real SoC scenarios / MITRE ATT&CK / Python + Pandas

This repository brings together Threat Hunting notebooks developed for investigating, detecting, and understanding suspicious behavior in enterprise environments.
The objective is to provide real examples, applicable to SOCs, Blue Teams and professionals who want to evolve in behavior-based detection, using Python and structured data.

🚀 Goals

✔ Demonstrate how a SOC analyst investigates threats in a practical way
✔ Apply Threat Hunting techniques on real datasets
✔ Map malicious behavior using MITRE ATT&CK
✔ Use Python, Pandas and exploratory analysis to find anomalies
✔ Serve as professional portfolio for cybersecurity / SOC positions

threat-hunting-notebooks/
│
├── datasets/
│ ├ ─ ─ auth_logs.csv
│ ├ ─ ─ dns_logs.csv
│ └ ─ ─ process_logs.csv
│
├── DNS_Tunneling_Detection.ipynb
├── Beaconing_Detection.ipynb
├── Rare_Processes.ipynb
Susp── Suspicious_Logins.ipynb
│
└── requirements.txt

Contents of Notebooks
1. DNS Tunneling Detection

Detects possible covert channels using DNS.

🛠 Applied techniques:

Entropy of domains

Unusual volume of requests

Rare domains

Behavioral Tunneling

MIT MITRE ATT&CK:

T1071.004-Exfiltration Over Unencrypted / Obfuscated Non-C2 Protocol

2. Beaconing Detection

Identification of periodic communication typical of C2 (Command and Control).

🛠 Applied techniques:

Autocorrelation

Periodicity analysis

Beacon signals

Grouping by timestamps

MIT MITRE ATT&CK:

T1071-Application Layer Protocol

T1008-Fallback Channels

3. Rare Processes Hunting

Search for rare or low-frequency processes - typical behavior of:

* malware
* lateral execution
* initial persistence

🛠 Applied techniques:

Behavioral Baseline

Frequency analysis

Detection of atypical processes

MIT MITRE ATT&CK:

T1059-Execution

T1106-Native API

4. Suspicious Logins

Detects suspicious patterns in authentication logs:

* Impossible Travel
* Login by leaked credential
* Repetitive attempts
* IP and geolocation anomalies

MIT MITRE ATT&CK:

T1110-Brute Force

T1078-Valid Accounts

🧠 Technologies Used

Python

Pandas

Jupyter Notebook

Plotly / Matplotlib (where applicable)

CSV datasets (simulated real logs)

▶️ How To Run
pip install-r requirements.txt
jupyter notebook


Open any notebook and load the datasets from the /datasets folder.

📌 Next Steps (Roadmap)

Add malicious PowerShell detection

Parse HTTP/Proxy logs

Create correlation dashboard

Enrichment via MITRE ATT & CK automatic

Final dashboard for SOC Tier 1 / Tier 2

🤝 Contributions

Pull requests, suggestions and issues are welcome.
This repository is a space for technical learning and sharing.

🎯 About Me

Gustavo Okamoto-Cybersecurity Analyst
Focus on: SOC / Threat Detection / Python Automation / Cloud Security (GCP / AWS)

LinkedIn: linkedin.com/in/gustavo-okamoto-de-carvalho-ti
GitHub: github.com/gustavo89587
