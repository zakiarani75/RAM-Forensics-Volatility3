# RAM Forensics & Memory Analysis using Volatility 3

## 📌 Project Overview
This repository contains the results of a comprehensive Memory Forensics investigation. The goal of this project was to analyze a volatile memory dump (RAM) to identify active processes, network connections, and potential security artifacts using the **Volatility 3** framework.

## 🛠 Tools & Environment
* **Analysis Framework:** Volatility 3
* **Operating System:** Kali Linux
* **Core Tools:** Python 3, Strings, Grep, and Catfish for file discovery.
* **Target Image:** Windows Memory Dump (.vmem/.raw)

## 🔍 Investigation Steps
1.  **Image Identification:** Determined the operating system profile for the memory dump.
2.  **Process Analysis:** Scanned the memory for running processes using `windows.pslist` and `windows.pstree` to identify any suspicious activity.
3.  **Network Activity:** Analyzed active network connections using `windows.netstat` to find any unauthorized remote communication.
4.  **Data Carving:** Used `strings` and pattern matching to extract sensitive information and hidden commands from the raw data.
5.  **Artifact Extraction:** Extracted registry hives and focused on security-related system logs.

## 📁 Repository Structure
* **forensics_results.txt:** Detailed output of all Volatility plugins executed during the analysis.
* **Final_Memory_Analysis.txt:** A summarized report highlighting the most critical memory findings.
* **commands_log.txt:** A step-by-step log of the terminal commands used throughout the investigation.

## 💡 Key Findings
* Successfully identified the parent-child relationship of active processes.
* Identified network sockets and IP addresses associated with the system at the time of the dump.
* Extracted readable strings that provided insight into user activity.

---
**Author:** Zakia Rani  
**Field:** Cyber Security / Digital Forensics

