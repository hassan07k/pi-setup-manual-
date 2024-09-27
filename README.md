# what you need to do when you start up a new pi
1. choose which language you want the pi to be

2. connect to your wife or use ethernet kable

3. the system wil ask you where are you so just choose your city or country

4. system will ask questions about you for example your name, your comuters name, make a  username and make a password

5. after that it will take a while to load to install it in

# after you get in the pi open termninal and do these commands to get started!

1. look after and install updates to all the programs that are installed
a. sudo apt update (look after updates)
b. sudo apt update (install updates)

2. skur på ssh

a. sudo apt install openssh-server (installing SSH-servers)
b. sudo systemctl enable (will do that SSH turns on startup)
c. sudo systemctl start ssh (starts SSH here and now)

5. find your ip - you will need it when you gonna use SSH
a. ip a 
b. if you have ethernet, will ip show beside eth0: line. if you only have wirless, vil ip show beside wlan0: line. ip-address is normally 10.2.2.x or something that looks like that (where x is there gonna be another number between 2 and 254)

6. install git, python and mariaDB
a. sudo apt install python3-pip
b. sudo apt install git
c. sudo apt install mariadb-server
sudo mysql_secure_installtion

7. new database-user and put correct rights
