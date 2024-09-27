## what you need to do when you start up a new pi
1. Choose which language you want the pi to be

2. Cennect to your wifi or use ethernet cable

3. The system wil ask you where are you so just choose your city or country

4. System will ask questions about you for example your name, your comuters name, make a  username and make a password

5. After that it will take a while to load to install it in

 ## after you get in the pi open termninal and do these commands to get started!

 1. Look after and install updates to all the programs that are installed

 1. A sudo apt update (look after updates)
 2. B sudo apt update (install updates)

2. Skur på ssh

1. A sudo apt install openssh-server (installing SSH-servers)
2. B sudo systemctl enable (will do that SSH turns on startup)
3. C sudo systemctl start ssh (starts SSH here and now)

5. Find your ip - you will need it when you gonna use SSH

1. A ip a 
2. B if you have ethernet, will ip show beside eth0: line. if you only have wirless, vil ip show beside wlan0: line. ip-address is normally 10.2.2.x or something that looks like that (where x is there gonna be another number between 2 and 254)

6. Install git, python and mariaDB

1. A sudo apt install python3-pip
2. B sudo apt install git
3. C sudo apt install mariadb-server
sudo mysql_secure_installtion

7. Add a new database user and set the correct permissions:
a. Log into MariaDB:

i. sudo mariadb -u root

b. Create a new user:

i. CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';

c. Grant the new user privileges:

i. GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost' IDENTIFIED BY 'password';

d. Update privileges:

i. FLUSH PRIVILEGES;

8. Install other software you need. For example, VS Code, another browser, Wireshark, Nmap, etc.
a. If you have trouble with VS Code, download the .deb file for arm64 from VS Code Linux Setup. Navigate to the folder where you downloaded the file.

b. Type sudo apt install ./code and press Tab, then Enter.

9. Run sudo apt update and sudo apt upgrade again.
Control the machine from your laptop using SSH
In the future, you can control the Pi from your laptop using SSH, for example, in CMD or PowerShell. To connect using SSH from your laptop, type:

ssh username@ip

(replace username and ip with your details)

PS: Turn off the machine with sudo shutdown now and wait a little before disconnecting the power 😊.

What is "sudo"?
"Sudo" stands for "superuser do" and gives you the rights to execute commands that require admin privileges. This means you can do anything on the machine, but it also means you can cause significant damage. Be especially careful if you use sudo when deleting or moving things!


