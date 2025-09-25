# 🧾 osTicket Installation Guide

## ✅ System Requirements

### Server:
- OS: Linux (Ubuntu/CentOS), Windows, or macOS
- Web Server: Apache or Nginx
- PHP: 7.4 – 8.1
- MySQL: 5.5+ or MariaDB

### PHP Extensions:
- mysqli
- gd
- imap
- xml
- intl
- mbstring
- json
- curl
- gettext

---

## ✅ Step 1: Install Required Software

### On Ubuntu/Debian:
```bash
sudo apt update
sudo apt install apache2 mysql-server php php-mysqli php-imap php-gd php-intl php-xml php-mbstring php-curl php-gettext unzip
```

![Installing Packages](images/install-packages.png)

### On Windows:
- Install XAMPP or WAMP (includes Apache, PHP, MySQL).
- Enable required PHP extensions in `php.ini`.

![Enable PHP Extensions](images/enable-php-extensions.png)

---

## ✅ Step 2: Download osTicket

- Go to: https://osticket.com/download
- Download the latest release (.zip)
- Extract to your web server root:
  - Linux: `/var/www/html/osticket`
  - Windows: `C:\xampp\htdocs\osticket`

![osTicket Download Page](images/osticket-download.png)

---

## ✅ Step 3: Create MySQL Database

```sql
CREATE DATABASE osticket;
CREATE USER 'ostuser'@'localhost' IDENTIFIED BY 'securepassword';
GRANT ALL PRIVILEGES ON osticket.* TO 'ostuser'@'localhost';
FLUSH PRIVILEGES;
```

![Create Database](images/create-database.png)

---

## ✅ Step 4: Set Permissions (Linux Only)

```bash
sudo chown -R www-data:www-data /var/www/html/osticket
sudo chmod -R 755 /var/www/html/osticket
```

![Set Permissions](images/set-permissions.png)

---

## ✅ Step 5: Start Web-Based Installer

- Open browser and go to:
  - `http://localhost/osticket`
- Follow the on-screen steps:
  - Check server requirements
  - Enter MySQL credentials
  - Set up Admin user

![Web Installer Step 1](images/web-installer-start.png)
![Web Installer Step 2](images/web-installer-config.png)

