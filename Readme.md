# Windows Memory Forensics & Artifact Extraction

This project demonstrates professional-grade memory forensics techniques using **Volatility 3** and advanced **Linux Data Carving** tools on a raw memory dump (`myram.raw`).

---

## 🛠️ Analysis Tools & Environment

* **Platform:** Kali Linux
- **Core Framework:** Volatility 3
- **Data Carving:** Strings, Grep (Regex based extraction)
- **Target File:** `myram.raw` (Windows Memory Image)

---

## 📂 Key Investigation Steps & Terminal Screenshots

### 1. Forensic Email Extraction
Using Regular Expressions (Regex) to carve out communication traces from the volatile memory.

#### Screenshot: Carved Emails
Here is the command output showing extracted developer emails from raw memory:
(image_6.png)

* **Key Result:** Successfully extracted emails (e.g., *byronimo@gmail.com*, *devel@kali.org*).

### 2. User Activity & Directory Mapping
Identifying local user artifacts and directory structures to verify the system owner.

#### Screenshot: Zakia Profile Traces
Output showing local home directories and metadata linked to user 'zakia':
(image_7.png)

* **Key Result:** Traced home directories and application files linked to profile `/home/zakia`.

### 3. System Integrity & Error Audit
Hunting for system-level alerts and session errors to identify crashes or security breaches.

#### Screenshot: Security & Error Flags
Here we see stack overflow and grub errors found in memory:
(image_8.png)

* **Key Result:** Identified stack overflow detections and parity errors.

### 4. Web Traffic Discovery
Extracting HTTP/HTTPS service traces to understand the network footprint.

#### Screenshot: Web Traffic Analysis
Captured HTTP headers and protocol instances:
(image_9.png)

* **Key Result:** Captured web server headers and exceptions.

---

## 📊 Investigation Conclusions

- Successfully recovered sensitive email artifacts from raw memory.
- Mapped out the user's local environment and recent file activity.
- Identified critical system errors that occurred during the session.

---
**Investigator:** Zakia Rani  
**Specialization:** Cyber Security & Digital Forensics

