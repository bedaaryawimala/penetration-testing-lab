# Port scanning
reconnaissance towards target to check open ports and available services

command

nmap -sS -p 1-100 192.168.221.130

service/version scan

nmap -sS -sV 192.168.221.130

Expected results:
  - traffick caught by suricata
  - port scan alerts show up
  - event can be seen from kibana
