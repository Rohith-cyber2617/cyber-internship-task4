# Findings Analysis - Firewall Rule Implementation and Testing

## **Initial State**
- Telnet service was **enabled** and allowed connections on port 23.
- Connection to `127.0.0.1:23` was successful before firewall blocking.

## **Firewall Rule Effect**
- Created a **TCP inbound firewall rule** specifically for port 23.
- Rule applied to **all network profiles**: Domain, Private, Public.

## **Final State**
- After applying the rule, all Telnet connection attempts failed with:
