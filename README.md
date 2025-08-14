# Task 7: Monitor System Resources Using Netdata

## Objective
Install **Netdata** to monitor and visualize system & application performance metrics in real-time.

---

## Tools Used
- **Netdata** (Free, Open-source Monitoring Tool)
- **Docker**

---

## Steps to Run

### Option 1: Run with Docker
```bash
docker run -d \
  --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
Option 2: Run with Docker Compose
docker compose up -d
Access the Dashboard
Open your browser and go to:
http://localhost:19999
Replace localhost with your server IP if running remotely.
Metrics You Can Monitor
CPU usage
Memory utilization
Disk I/O
Docker containers performance
Network activity
System processes
Logs Location
/var/log/netdata
Deliverables
Screenshot of the Netdata dashboard showing running metrics:
References
Netdata Documentation
Netdata GitHub
