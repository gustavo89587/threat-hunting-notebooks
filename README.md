🛡️ Threat Hunting Notebooks
Análises, detecções e investigações em cenários reais de SOC | MITRE ATT&CK | Python + Pandas

Este repositório reúne notebooks de Threat Hunting desenvolvidos para investigação, detecção e entendimento de comportamentos suspeitos em ambientes corporativos.
O objetivo é fornecer exemplos reais, aplicáveis a SOCs, Blue Teams e profissionais que desejam evoluir em detecção baseada em comportamento, usando Python e dados estruturados.

🚀 Objetivos

✔ Demonstrar como um analista SOC investiga ameaças de forma prática
✔ Aplicar técnicas de Threat Hunting em datasets reais
✔ Mapear comportamento malicioso usando MITRE ATT&CK
✔ Utilizar Python, Pandas e análise exploratória para encontrar anomalias
✔ Servir como portfólio profissional para posições de Cybersecurity / SOC

threat-hunting-notebooks/
│
├── datasets/
│   ├── auth_logs.csv
│   ├── dns_logs.csv
│   └── process_logs.csv
│
├── DNS_Tunneling_Detection.ipynb
├── Beaconing_Detection.ipynb
├── Rare_Processes.ipynb
├── Suspicious_Logins.ipynb
│
└── requirements.txt

Conteúdo dos Notebooks
1. DNS Tunneling Detection

Detecta possíveis canais encobertos utilizando DNS.

🛠 Técnicas aplicadas:

Entropia de domínios

Volume incomum de requisições

Domínios raros

Tunneling comportamental

🧩 MITRE ATT&CK:

T1071.004 – Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol

2. Beaconing Detection

Identificação de comunicação periódica típica de C2 (Command and Control).

🛠 Técnicas aplicadas:

Autocorrelação

Análise de periodicidade

Sinais de beacon

Agrupamento por timestamps

🧩 MITRE ATT&CK:

T1071 – Application Layer Protocol

T1008 – Fallback Channels

3. Rare Processes Hunting

Busca por processos raros ou com baixa frequência — comportamento típico de:

• malware
• execução lateral
• persistência inicial

🛠 Técnicas aplicadas:

Baseline comportamental

Frequency analysis

Detecção de processos atípicos

🧩 MITRE ATT&CK:

T1059 – Execution

T1106 – Native API

4. Suspicious Logins

Detecta padrões suspeitos em logs de autenticação:

• Impossible Travel
• Login por credencial vazada
• Tentativas repetitivas
• Anomalias de IP e geolocalização

🧩 MITRE ATT&CK:

T1110 – Brute Force

T1078 – Valid Accounts

🧠 Tecnologias Utilizadas

Python

Pandas

Jupyter Notebook

Plotly / Matplotlib (quando aplicável)

CSV datasets (logs reais simulados)

▶️ Como Executar
pip install -r requirements.txt
jupyter notebook


Abra qualquer notebook e carregue os datasets da pasta /datasets.

📌 Próximos Passos (Roadmap)

Adicionar detecção de PowerShell malicioso

Analisar logs de HTTP/Proxy

Criar painel de correlação

Enriquecimento via MITRE ATT&CK automático

Dashboard final para SOC Tier 1/Tier 2

🤝 Contribuições

Pull requests, sugestões e issues são bem-vindos.
Este repositório é um espaço para aprendizado e compartilhamento técnico.

🎯 Sobre Mim

Gustavo Okamoto — Cybersecurity Analyst
Foco em: SOC | Threat Detection | Python Automation | Cloud Security (GCP/AWS)

LinkedIn: linkedin.com/in/gustavo-okamoto-de-carvalho-ti
GitHub: github.com/gustavo89587

