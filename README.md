# OpenCanaryd Honeypot on Ubuntu
This project sets up a honeypot environment using OpenCanaryd on Ubuntu to attract and monitor malicious activities from potential attackers. Email notifications alert you promptly when attacks occur.

## Prerequisites

- Ubuntu system
- Root or sudo privileges
- Email server/service (e.g., Gmail, SMTP)
- Installation

1. Update: sudo apt update && sudo apt upgrade
2. Install OpenCanaryd: sudo apt install opencanaryd
3. Configure:
  - Edit /etc/opencanaryd/opencanaryd.conf (e.g., sudo nano /etc/opencanaryd/opencanaryd.conf)
    - Configure services (SSH, VNC, RDP), logging, and email alerting (server details, recipients).
4. Enable and Start:
```
sudo systemctl enable opencanaryd
sudo systemctl start opencanaryd
Verification
```

Check service status: sudo systemctl status opencanaryd
Access web interface (http://localhost:8000 by default, if enabled).
Monitoring

Review logs for detailed attack information.
Email alerts provide basic notification.
