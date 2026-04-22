# Flood Simulation
Simulate flood attack to produce abnormal traffic.

SYN flood to SSH port

sudo hping3 -S --flood -p 22 192.168.221.130

SYN flood to HTTP port

sudo hping3 -S --flood -p 80 192.168.221.130

Expected results:
  - custom rule and built-in suricata alert show up
  - event can be seen in kibana
