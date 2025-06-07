# 🚀 Monitor System Resources Using Netdata

## 📌 Task Overview
Installed and ran Netdata inside a Docker container to monitor system resource usage (CPU, RAM, Disk, Network, etc.) in real-time. Explored the Netdata dashboard to visualize performance metrics.

## 🛠 Tools Used
- Docker (v28.1.1)  
- Netdata (Official Docker Image)  
- Docker Desktop  
- PowerShell Terminal  

## 📂 Files Included
- `README.md`: Documentation for the task.  
- `screenshots/`: Folder containing screenshots of the dashboard and terminal outputs.  

## 🚀 Steps Followed
- Verified Docker installation using `docker --version`.  
- Ran Netdata container with `docker run -d --name=netdata -p 19999:19999 netdata/netdata`.  
- Confirmed container was running using `docker ps`.  
- Accessed the dashboard at [http://localhost:19999](http://localhost:19999).  
- Explored CPU, memory, disk, network, and Docker container metrics.  
- Viewed Netdata logs via `docker exec -it netdata cat /var/log/netdata/error.log`.  

## 🔗 Live Dashboard Access
Open [http://localhost:19999](http://localhost:19999) in your browser to view system metrics live.

## ✅ Status
Task Completed Successfully!
