# Penetration Testing Lab
Penetration testing is done from kali as attacker to ubuntu live server. The goal is to prove that the mini SOC lab can catch and display the attack activity from host and network telemetry.

The penetration testing includes:
  - port scanning
  - brute force
  - web probing
  - flood

Result shows that every activity can be detected wether it's from custom rule suricata, built-in alert suricata, or log host in kibana.

# Topology
the structures for this soc lab is the same as the one in elastic-soc-lab repo with the addition of suricata and its custom rule.

Ubuntu live server
  - Elasticsearch
  - Kibana
  - Fleet Server
  - Elastic Agent
  - Suricata IDS
  - Nginx for web probing target

Kali Linux
  - Elastic Agent
  - Nmap
  - Hydra
  - Nikto
  - hping3

# Additional Notes
events can be seen from eve.json by using:

tail -f /var/log/suricata/eve.json | grep -a '"event_type":"alert"'

(that command will only show the suricata alert response to the attack)

to see all of the events, use:

tail -f /var/log/suricata/eve.json
