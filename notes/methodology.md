# Methodology - Firewall Rule Implementation and Testing

## 1. Environment Setup
- Used **Windows 10 VM** inside VMware.
- Verified Telnet Client/Server is installed via:
  - Control Panel → Programs → Turn Windows features on or off.

## 2. Enabling Telnet Service
1. Press `Win + R` → type `services.msc`.
2. Locate **Telnet** service → Right-click → **Properties**.
3. Set **Startup type** to **Automatic** and click **Start**.

## 3. Testing Telnet Connection (Before Firewall Block)
- Open Command Prompt and run:
  ```
  telnet 127.0.0.1 23
  ```
- If connected successfully (blank screen or login prompt), it means port 23 is open.

## 4. Blocking Port 23 Using Firewall
1. Open **Control Panel → Windows Defender Firewall → Advanced Settings**.
2. Go to **Inbound Rules → New Rule**.
3. Select **Port** → **TCP** → Specific port: `23`.
4. Choose **Block the connection** → Apply to **Domain, Private, Public** → Name rule `Block Telnet`.

## 5. Testing Telnet Connection (After Firewall Block)
- Run the same command:
  ```
  telnet 127.0.0.1 23
  ```
- Expected output:
  ```
  Could not open connection to the host, on port 23: Connect failed
  ```

---

**Result:** The firewall rule successfully blocked access to the Telnet service.
