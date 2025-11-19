# Firewall-
Configure Firewall Rules to Allow or Block Network Traffic


---

📌 Objective

To configure basic firewall rules on either Windows Firewall or UFW (Linux), test them, and document the applied configurations.


---

🧰 Tools Used

Windows Defender Firewall
or

UFW (Uncomplicated Firewall) on Linux/Ubuntu



---

🚀 Steps I Followed

1. Checked Existing Firewall Status

For Linux:

sudo ufw status verbose

For Windows:

Opened Windows Defender Firewall

Viewed Inbound/Outbound Rules



---

2. Added Rule to Block a Port

Example (Block Telnet on Port 23):

Linux (UFW):

sudo ufw deny 23

Windows:

Created a new Inbound Rule

Set port = 23

Action = Block



---

3. Allowed SSH (Linux only)

sudo ufw allow 22


---

4. Tested the Rules

Used telnet localhost 23 or nc to simulate traffic

Verified the port was blocked as expected



---

5. Removed the Test Rule

sudo ufw delete deny 23

(or deleted rule in Windows Firewall)
