fail2ban
---------
Protects SSH from repeated failed login attempts

/jail.local
- Configuration file, located in /etc/fail2ban/jail.local

sudo fail2ban-client status sshd
- View the status of the sshd jail

sudo fail2ban-client set sshd unbanip (ip)
- Unban an IP from the sshd jail

sudo systemctl restart fail2ban
- Apply changes made in config

sudo journalctl -u fail2ban -f
- View fail2ban logs in real time
