# Monitoring with Netdata

This project demonstrates how to monitor system resources and application performance using Netdata, running inside a Docker container. The guide includes setup, usage, and log access instructions, along with example screenshots and a project report.

## Table of Contents
- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Cloning the Repository](#cloning-the-repository)
- [Running Netdata with Docker](#running-netdata-with-docker)
- [Accessing the Netdata Dashboard](#accessing-the-netdata-dashboard)
- [Accessing Netdata Logs](#accessing-netdata-logs)
- [Stopping and Removing Netdata](#stopping-and-removing-netdata)
- [Project Report](#project-report)

## Project Overview
Netdata is a free, open-source monitoring tool that provides real-time insights into system and application metrics. This project uses Docker to run Netdata and visualize metrics such as CPU, memory, disk, and network usage.

## Prerequisites
- Windows OS
- [Docker Desktop](https://www.docker.com/products/docker-desktop) installed and running
- Git installed

## Cloning the Repository
Open PowerShell and run:
```powershell
git clone https://github.com/Renuu007/Monitoring-with-Netdata
cd Monitoring-with-Netdata
```

## Running Netdata with Docker
Start Netdata in a Docker container:
```powershell
docker run -d --name=netdata -p 19999:19999 netdata/netdata
```

## Accessing the Netdata Dashboard
Open your browser and go to:
```
http://localhost:19999
```
You will see real-time system metrics and dashboards.

## Accessing Netdata Logs
To view logs inside the Netdata container:
```powershell
docker exec -it netdata bash
cd /var/log/netdata
ls
cat error.log  # or tail -n 50 error.log
exit
```

## Stopping and Removing Netdata
To stop and remove the Netdata container:
```powershell
docker stop netdata
docker rm netdata
```

## Project Report
See `Netdata_Report.md` for annotated screenshots and descriptions of the monitoring dashboards and log access steps.

---

Feel free to explore the Netdata dashboard, check logs, and customize your monitoring setup as needed!
