# 🚀 Task 7: Monitor System Resources Using Netdata

## ✅ Objective
To monitor system resource usage (CPU, RAM, Disk, Network, etc.) in real-time using Netdata running inside a Docker container.

---

## 🛠 Tools & Technologies Used
- Docker (v28.1.1)
- Netdata (Official Image)
- Docker Desktop (GUI)
- PowerShell (Terminal)

---

## 📋 Commands Used with Explanation

1. ### `docker --version`
   **Purpose:** Check if Docker is installed and view the installed version.

2. ### `docker run -d --name=netdata -p 19999:19999 netdata/netdata`
   **Purpose:** Run the Netdata container in the background.
   - `-d`: Run container in detached mode (background)
   - `--name=netdata`: Assign the container a name `netdata`
   - `-p 19999:19999`: Map local port 19999 to the container’s port 19999
   - `netdata/netdata`: The Docker image to run

3. ### `docker ps`
   **Purpose:** Show all currently running containers. Helps to confirm if Netdata is running.

4. ### `docker exec -it netdata cat /var/log/netdata/error.log`
   **Purpose:** Run a command inside the running container.
   - `exec`: Execute a command in the container
   - `-it`: Interactive terminal mode
   - `netdata`: Name of the container
   - `cat /var/log/netdata/error.log`: View Netdata's error log (used for debugging if needed)

5. ### Open in browser  
🔗 [http://localhost:19999](http://localhost:19999)  
**Purpose:** View the real-time Netdata monitoring dashboard.

---

## 📸 Screenshots Included
- ✅ Netdata live dashboard  
- ✅ Terminal commands output  
- ✅ Docker Desktop view showing running containers

All screenshots are in the `screenshots/` folder.

---

## 📂 Files in This Repo
- `README.md` – This file  
- `screenshots/` – Folder with all screenshot images

---

## 🔍 What I Learned
- How to install and run a containerized app using Docker  
- How to expose container ports to access services on localhost  
- How to verify and manage running containers using Docker CLI and Desktop  
- How to read logs from a container  

---

## ✅ Task Status
**✔ Completed**

---

## 🔗 Live Dashboard Access (Localhost)
Visit [http://localhost:19999](http://localhost:19999) in your browser to monitor system stats in real time.

---

## 📥 GitHub Submission Checklist
- [x] Created a new GitHub repo for Task 7  
- [x] Added `README.md`  
- [x] Added `screenshots/` folder  
- [x] Pushed everything to GitHub  
