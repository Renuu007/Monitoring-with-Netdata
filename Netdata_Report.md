# Netdata Monitoring Project Report

## Snapshot 1: Accessing Netdata Logs in the Container

![Netdata Logs Terminal](images/image-1.png)

**Description:**
This screenshot shows the process of accessing the Netdata log files inside the Docker container. The user enters the container using `docker exec -it netdata bash`, navigates to `/var/log/netdata`, and lists the available log files. These logs are useful for troubleshooting and monitoring Netdata's internal operations.

---

## Snapshot 2: Netdata Dashboard - System Metrics Overview

![Netdata Dashboard Metrics](images/image-2.png)

**Description:**
This screenshot displays the main Netdata dashboard, which provides real-time monitoring of system resources. Key metrics such as CPU usage, RAM usage, disk reads/writes, and network activity are visualized. The dashboard allows users to quickly assess the health and performance of the system.

---

## Snapshot 3: Netdata Custom Dashboard - RAM Usage Details

![Netdata Custom Dashboard RAM](images/image-3.png)

**Description:**
This screenshot shows a custom dashboard in Netdata focusing on system RAM usage. The chart visualizes memory allocation over time, including free, used, cached, and buffer memory. This helps in understanding memory consumption patterns and identifying potential issues.

---

## Summary

These snapshots demonstrate the setup, monitoring, and analysis capabilities of Netdata using Docker. The project covers accessing logs, visualizing key system metrics, and exploring detailed resource usage through custom dashboards.
