# Dizzy-DNS

A Python script for DNS spoofing using netfilterqueue and Scapy.

## Prerequisites

- Python 3
- Install required modules:
  ```bash
  pip install netfilterqueue
  
#Usage
Set up iptables to redirect DNS traffic to the tool:

iptables -I INPUT -j NFQUEUE --queue-num 0
Run the DNS spoofer with the specified target and redirection website:

python dns_spoofer.py -s <target_website> -r <redirect_website>
Replace <target_website> with the website you want to spoof, and <redirect_website> with the website to which you want to redirect the user.

Monitor DNS requests and observe the spoofing process.

#Example

python dns_spoofer.py -s example.com -r malicious-website.com

Notes
This tool currently works for DNS requests on localhost.

Disclaimer
This tool is intended for educational and ethical use only. Ensure compliance with legal regulations and obtain proper authorization before using it in any environment.
