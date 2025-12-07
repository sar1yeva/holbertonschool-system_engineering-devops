Web infrastructure design
-------
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/89c94a8b-0dc6-4360-965e-453074e12f98" />

-----
General
-----
1️⃣ Web Stack Diagram (LAMP Example)

A LAMP stack is a common web stack:


<img width="1941" height="1104" alt="image" src="https://github.com/user-attachments/assets/1f2db2eb-8bcf-4bfe-aa66-7e63a73aa3fb" />

<img width="800" height="465" alt="image" src="https://github.com/user-attachments/assets/7deb6dec-fa11-4729-9d63-f0331dc7b39d" />



Clients / Users: Devices like browsers or mobile apps requesting web pages or data.

Load Balancer / Reverse Proxy: Distributes traffic to multiple web servers. Improves redundancy and prevents a single server from being overwhelmed.

Web Server (Apache/Nginx): Handles HTTP requests, serves static content, and forwards dynamic requests to the application layer (PHP in LAMP).

Application Layer (PHP): Processes business logic, interacts with databases, generates dynamic content.

Database (MySQL/MariaDB): Stores persistent data (users, posts, transactions). Can be set up in master-slave replication for redundancy.

Storage / Backup: Keeps files, logs, and backups. Ensures data recovery in case of failure.

---------
2️⃣ System Redundancy
-------
<img width="581" height="489" alt="image" src="https://github.com/user-attachments/assets/eadeccde-865e-452b-a47a-5f7134c67900" />

Redundancy ensures that if one component fails, the system continues working:

Web Servers: Use multiple servers behind a load balancer → if one goes down, traffic is routed to the others.

Database: Use replication or clustering → master-slave or master-master setups prevent a single point of failure.

Storage: Backup data regularly → allows recovery if storage fails.

Network: Multiple network paths / ISPs → avoids network downtime.

--------
3️⃣ Acronyms
---------

LAMP:
Linux (OS)
Apache (Web Server)
MySQL/MariaDB (Database)
PHP (Programming Language)

SPOF: Single Point of Failure → a component whose failure stops the entire system.

QPS: Queries Per Second → measures how many database or web requests a system handles per second.


<img width="1200" height="675" alt="image" src="https://github.com/user-attachments/assets/bb4061af-ec10-4d6b-a54a-7624716c6783" />






