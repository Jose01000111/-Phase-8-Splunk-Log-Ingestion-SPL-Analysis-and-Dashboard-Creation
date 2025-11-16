# 🚀Phase 8: Splunk Log Ingestion, SPL Analysis, and Dashboard Creation

In this lab, I got hands-on with Splunk Enterprise running inside Docker. I uploaded a sample log, practiced SPL queries to explore and analyze the data, and built a custom dashboard to visualize total logs, top hosts, and event trends over time. This lab gave me a practical understanding of Splunk's search capabilities and dashboard creation workflow.  

---

# 🚀 Start Splunk Container
I launched Splunk Enterprise inside a Docker container on my Windows 11 host to create an isolated environment for testing. Running Splunk in Docker makes it easy to reset, manage, and experiment without affecting my main system.  

<img width="1271" height="248" alt="hHwH9QI" src="https://github.com/user-attachments/assets/5bdc177b-a654-447c-a63c-d89d5b993383" />

>- 🐳 **Docker** — container platform to run Splunk in an isolated environment  
>- 🖥️ **Windows 11** — host OS for Docker  
>- 🖱️ **Splunk Enterprise** — SIEM tool for log management, searching, and visualization  

---

# 📂 Upload Sample Log
I prepared a sample log file (`sample2.log`) and copied it into the Docker container. Then I uploaded it into Splunk using the **Add Data** wizard. I defined the source type as `syslog` so Splunk could properly parse the events and stored the events in the `os_logs` index.  

<img width="706" height="133" alt="hIXGp72" src="https://github.com/user-attachments/assets/8bb801a7-f273-4184-a23e-822ed0c63708" />

<img width="695" height="235" alt="57YP7eZ" src="https://github.com/user-attachments/assets/1af5fa23-957c-4df9-928a-a2961f6ede23" />

>- 🗂️ **Log ingestion** — process of bringing log files into Splunk for indexing and searching  
>- 🏷️ **Index (`os_logs`)** — storage location for all events from this log  
>- 📝 **Source type (`syslog`)** — Splunk parser type defining how the log data is interpreted  

---

# 🔍 SPL Practice
I ran multiple searches using Splunk Processing Language (SPL) to explore and analyze the ingested log data. This included filtering events, aggregating by host, and creating time-based visualizations to understand event trends. Practicing SPL is essential to mastering Splunk for security monitoring and analysis.  

<img width="950" height="161" alt="KZZdCBC" src="https://github.com/user-attachments/assets/cd5b030b-e0af-4ea5-aa06-1a4eadc0872b" />

---

<img width="972" height="208" alt="kyKB9CS" src="https://github.com/user-attachments/assets/cf32203d-bf7b-4a4d-8cff-68e6ad501a87" />

>- 🔎 **Search** — queries to retrieve events from Splunk indexes  
>- 📊 **Stats & top commands** — aggregate data (like event counts per host) and identify most frequent items  
>- 🕒 **Timechart** — create visual graphs of event volume over time  
>- ✏️ **Filter & keyword search** — narrow down logs by specific terms like `error`  

---

# 📊 Dashboard Creation
I created a custom Splunk dashboard to visualize the data I analyzed. The dashboard included three panels: Total Logs, Top Hosts, and Log Volume Over Time. Each panel used the SPL queries I practiced and displayed the results using appropriate visualizations (Statistics Table and Line Chart). Building dashboards helps make data analysis easier to interpret at a glance.  

<img width="583" height="546" alt="X1HmWUB" src="https://github.com/user-attachments/assets/f911f76b-15f5-4ea5-b327-725f23fe7716" />

---

<img width="753" height="353" alt="hPbQVC6" src="https://github.com/user-attachments/assets/2dd81619-4d7e-44d2-aabc-54ae902a774f" />

---

<img width="755" height="377" alt="0FzV95e" src="https://github.com/user-attachments/assets/f1e3448f-becc-4d02-acee-8bc3131f6669" />

>- 📈 **Dashboard** — centralized view of multiple searches and visualizations  
>- 🖼️ **Panels** — individual charts or tables for each SPL query  
>- 🧰 **Visualizations** — used **Statistics Table** for counts and **Line Chart** for time trends  
>- 💡 **Practical tip** — dashboards let you quickly detect anomalies and trends in log data  

---

# 🛑 Shutdown Docker
At the end of the lab, I safely stopped the Splunk container to free system resources and preserve my work for the next session. I confirmed the container was stopped and then closed Docker Desktop. This ensures a clean environment for future labs.  

<img width="492" height="66" alt="HxQIHXG" src="https://github.com/user-attachments/assets/e703b628-bc8a-4d28-8476-e1076c366e79" />


>- ⏹️ **docker stop splunk-lab** — gracefully stops the running container  
>- 🔍 **docker ps -a** — verify container is stopped (status = Exited)  
>- 🖥️ **Docker Desktop quit** — fully closes the Docker application  

---

✅ **Lab complete:** I successfully ran Splunk in Docker, uploaded and ingested logs, practiced SPL queries, built a functional dashboard, and safely shut down my environment. This lab strengthened my practical Splunk skills for SIEM and log analysis workflows.
