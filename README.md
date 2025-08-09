# Cyber Internship – Task 4: Firewall Setup & Testing

## Objective
Configure and test basic firewall rules to allow or block network traffic.

## Tools Used
- **Windows Firewall with Advanced Security**
- Command Prompt (`telnet`) for testing
- UFW (Linux equivalent commands documented in `notes/methodology.md`)

## Methodology
1. Viewed existing firewall rules.
2. Created inbound rule to block TCP port 23 (Telnet).
3. Tested the block using `telnet`.
4. Documented Linux equivalent commands for UFW.
5. Removed the test rule to restore original state.

## Screenshots
| Step | Image |
|------|-------|
| Initial Rules | ![Initial Rules](screenshots/initial_rules.png) |
| Block Telnet Rule | ![Block Telnet](screenshots/block_telnet.png) |
| Testing Block | ![Test Block](screenshots/test_block.png) |
| Rule Removal | ![Remove Rule](screenshots/remove_rule.png) |

## Key Learnings
- Difference between **inbound** and **outbound** rules.
- Why blocking insecure ports (e.g., Telnet) is important.
- Linux UFW makes firewall rule management simple with commands like:
  ```bash
  sudo ufw allow 22/tcp
  sudo ufw deny 23/tcp
  sudo ufw status
