# Setting-up Database di AWS Ec2 menggunakan MariaDb

1. Aktifkan Instance AWs Ec2
2. Remote Instance Via Open SSH Powershell / putty
3. Patching OS (sudo apt-get update && sudo apt-get upgrade)
4. Install MariaDb (sudo apt install mariadb-server -y)
5. Cek Status MariaDb (systemctl status mariadb)
![alt text]({71D9B816-D2B6-49C9-9A30-CED5794164C7}.png)

6. Test Default Setting database server login sudo mysql -u root -p
![alt text]({C6A1207B-CD0C-42CC-9040-EF7A9F576EDA}.png)


7. Hardening Database Server sudo mysql_secure_installation
- Change the password for the root user = Y
- Remove anonymous users = Y
- Disallow root login remotely = Y
- Remove test database and access to it = Y
- Reload privilege tables = Y
![alt text]({2369EEBD-6AD1-428A-8D14-0818DD54285A}.png)

8. Create DB untuk Website Company Profile
- Login sebagai root
- Create DB nama dbcompro_NIM => CREATE DATABASE dbcompro_NIM;
- Create User dengan nama = usrcompro_NIM dan password = [PASSWORD] => CREATE USER 'usrcompro_NIM'@'localhost' IDENTIFIED BY '[PASSWORD]';
![alt text]({A5B1BAB1-84C4-485A-9A63-DDDB3A31ECBD}.png)

- Grant user akses ke DB yang baru dibuat => GRANT ALL PRIVILEGES ON dbcompro_NIM.* TO 'usrcompro_NIM'@'localhost';
- Flush privileges => FLUSH PRIVILEGES;
- exit;
- login sebagai usrcompro_NIM dan cek apakah bisa akses ke DB yang baru dibuat
![alt text]({A341875D-B70D-4748-ABE3-7495F07E1B61}.png)