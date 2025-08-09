# Cyber Internship - Task 4  
**Title:** Firewall Rule Implementation and Testing  
**Intern Name:** Rachapudi Rohith (Tony)  
**Task Objective:** Configure firewall rules to block a specific port (Telnet - Port 23) and verify its effectiveness.  

---

## 📌 Task Overview  
This task demonstrates how to:
1. Enable a Telnet service on the system.
2. Connect to it locally.
3. Block the connection using a Windows firewall rule.
4. Verify that the firewall rule is working.

---

## 🛠 Tools Used
- **Windows 10 VM** (inside VMware)
- **Windows Defender Firewall**
- **Telnet Client & Telnet Server** (Windows Features)

---

## 📂 Repository Structure

```
cyber-internship-task4/
│
├── notes/                              # Documentation and analysis
│   ├── methodology.md                  # Step-by-step firewall configuration process
│   └── findings_analysis.md             # Observations & conclusions
│
├── screenshots/                        # All captured screenshots from the task
│   ├── windows_defender.png
│   ├── initial_rules.png
│   ├── telnet_firewall_configuration.png
│   ├── type_of_firewall.png
│   └── firewall_successfully_blocked.png
│
│
└── README.md                           # Main documentation for the task
```

---
## 📸 Screenshots

Below are the captured screenshots for Task 4:

1. **Windows Defender**
   ![Windows Defender](screenshots/windows%20defender.png)

2. **Initial Rules**
   ![Initial Rules](screenshots/initial_rules.png)

3. **Telnet Firewall Configuration**
   ![Telnet Firewall Configuration](screenshots/telnet%20firewall%20configuration.png)

4. **Type of Firewall**
   ![Type of Firewall](screenshots/type%20of%20firewall.png)

5. **Firewall Successfully Blocked**
   ![Firewall Successfully Blocked](screenshots/firewall%20successfully%20blocked.png)

---

## 📑 Notes
Detailed methodology → [methodology.md](notes/methodology.md)  
Analysis of findings → [findings_analysis.md](notes/findings_analysis.md)  

---

## ✅ Conclusion
The test successfully showed that the firewall rule effectively blocked port 23, preventing Telnet access. This validates that firewall configurations can control network access to services.
