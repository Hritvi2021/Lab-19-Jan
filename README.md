# Lab-19-Jan

# Networking Basics – CLI Hands-On Lab
Primary: Linux CLI (Ubuntu / Amazon Linux)
1. Understand IP Addressing
2. Check IP Address & Interface Details
   Linux Command
   bash
   ip a / ifconfig
   
 <img width="1366" height="768" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/0e5d297b-29ac-4688-a4b5-8900b2c5e2a7" />

# We Can Observe :
. Interface name: eth0, ens33, wlan0
. IP address (IPv4)
. MAC address
. Interface state (UP / DOWN)

# Test Network Connectivity (Ping)
  Linux Command
  bash
  ping 2.2.2.2 / ping googel.com
# We Can Observe:
. Packet loss
. Response time (latency)
. DNS resolution (when using domain name)
# Stop ping
  ctrl + c

<img width="1366" height="768" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/a32342ac-21d2-462c-9b16-5697839fefa8" />

# Inspect Open Ports and Services
Linux Command
bash
netstat -tulnp / ss -tulnp
(t-TCP, u-UDP, l-Listening, n-Numeric Output, p-Process info)

<img width="1366" height="768" alt="Screenshot (29)" src="https://github.com/user-attachments/assets/d1717a4a-ca92-4b28-981c-d87321fd1eeb" />

# DNS Resolution
Linux Command
bash
nslookup google.com / dig google.com
# We Can Observe:
. DNS server used
. IP returned
. Query time

<img width="1366" height="768" alt="Screenshot (30)" src="https://github.com/user-attachments/assets/62284012-2fb4-4450-b50a-75448d13c721" />

# Trace Network Path
  Linux Command
  bash
  tracerout google.com
# We Can Observe:
. Number of hops
. Where latency increases
. Where packets drop  

<img width="1366" height="768" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/5f9a1370-ef73-41f9-9488-9efce58f252d" />

# Simulate Network Failure
Linux Command
bash
sudo ip link set eth0 down (Disable)
sudo ip link set eth0 up (Enable)



