# Brute Force
Simulate incorrect logins with incorrect passwords using hydra to cause detection on a network and host level

hydra command:

hydra -l beda -p salahpassword 192.168.221.130 ssh -s 22 -t 2 -V

Expected results:
  - Suricata gives brute force alert both in log and in kibana
  - event can be seen in kibana
