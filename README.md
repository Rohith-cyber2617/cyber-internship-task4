# Cyber Internship - Task 4  
**Title:** Firewall Rule Implementation and Testing  
**Intern Name:** Rachapudi Rohith (Tony)  
**Task Objective:** Configure firewall rules to block a specific port (Telnet - Port 23) and verify its effectiveness.  

---

## **📌 Task Overview**  
This task demonstrates how to:
1. Enable a Telnet service on the system.
2. Connect to it locally.
3. Block the connection using a Windows firewall rule.
4. Verify that the firewall rule is working.

---

## **🛠 Tools Used**
- **Windows 10 VM** (inside VMware)
- **Windows Defender Firewall**
- **Telnet Client & Telnet Server** (Windows Features)

---

## **📂 Repository Structure**
Task4/
│── README.md
│── notes/
│ ├── methodology.md
│ ├── findings_analysis.md
│── screenshots/
│ ├── telnet_enabled.png
│ ├── telnet_connected.png
│ ├── firewall_rule_added.png
│ ├── telnet_blocked.png

---

## **📷 Screenshots**
1. **Telnet Service Enabled**  
   ![Telnet Enabled](screenshots/telnet_enabled.png)

2. **Telnet Connected Before Firewall Block**  
   ![Telnet Connected](screenshots/telnet_connected.png)

3. **Firewall Rule Added for Port 23**  
   ![Firewall Rule Added](screenshots/firewall_rule_added.png)

4. **Telnet Connection Blocked**  
   ![Telnet Blocked](screenshots/telnet_blocked.png)

---

## **📑 Notes**
Detailed methodology → [methodology.md](notes/methodology.md)  
Analysis of findings → [findings_analysis.md](notes/findings_analysis.md)  

Could not open connection to the host, on port 23: Connect failed


---

### **Conclusion**
This experiment confirmed that Windows Firewall rules can effectively:
- Block access to a specific service by port number.
- Restrict connections both locally and remotely.

**Security Relevance:**  
- Blocking unused or vulnerable ports reduces the attack surface.
- Helps prevent unauthorized access to legacy services like Telnet.


---

## **✅ Conclusion**
The test successfully showed that the firewall rule effectively blocked port 23, preventing Telnet access. This validates that firewall configurations can control network access to services.
