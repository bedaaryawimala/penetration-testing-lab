# Web Probing
simulate peobing and web based enumeration on ubuntu server HTTP service 

HTTP access using:

curl http://192.168.221.130

Web probing using nikto:

nikto -h http://192.168.221.130

Expected results:
  - HTTP traffic caught by suricata
  - custom rule alerts show up
  - built-in HTTP alerts show up
  - event can be seen from kibana with the destination port 80
