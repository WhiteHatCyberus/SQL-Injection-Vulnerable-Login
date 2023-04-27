# SQL-Injection-Vulnerable-Login
**Status**: In Progress
![f1](https://user-images.githubusercontent.com/70995581/233904518-8eae5480-3388-43f3-bd9f-0741252dee91.png)
- This repo intends to help security researchers implement sql injection techniques on their local host or target system.
- The website is built using basic html, css and js , additionally with a mysql server in the backend to validate login. This is intended to be hosted on a Apache2 port 80 webserver.
- No sql injection handling methods are implemented so the hosted website is vulnerable to sql injecton.
> **Warning**: Do not use this website in a production environment, *for isolated simulation environments only*.

# Apache2 webserver setup:
- Apache2 is a Linux based webserver to host websites in port 80/8080 of host system.
- Installation: 
```bash
sudo apt install apache2 -y
```
- All website componenets to be hosted on Apache2 should be uploaded into the `/var/www/html/' folder.
- Check if apache2 is working. Run:
```bash
sudo systemctl start apache2
```
- Allow port 80 (http) to listen across the firewall:
```bash
sudo ufw allow 80/tcp
```
- Search `localhost` or `<ip_addr:80>` in your browser.
