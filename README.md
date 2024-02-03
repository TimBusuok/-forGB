1 mkdir Work
2 cd ~/Work
3 cat > home_animals
4 cat > silly_animals
5 cat home_animals silly_animals > animals
6 cat animals
7 mv animals mans_friends
8 cd mans_friends
9 ll
10cd ~
11 mkdir work_system
12 cd ~/Work
13 mv mans_friends ~/work_system
14 cd ~/work_system
15 ll
16 sudo wget https://dev.mysql.com/get/mysql-apt-config_0.8.23-1_all.deb
17 sudo dpkg -i mysql-apt-config_0.8.23-1_all.deb
18 sudo apt-get update
19 sudo apt-get install mysql-server
20 sudo wget https://download.docker.com/linux/ubuntu/dists/jammy/pool/stable/amd64/docker-ce-cli_20.10.13~3-0~ubuntu-jammy_amd64.deb
21 sudo dpkg -i docker-ce-cli_20.10.133-0ubuntu-jammy_amd64.deb
22 sudo dpkg -r docker-ce-cli


![Диаграмма](https://github.com/TimBusuok/-forGB/assets/129662995/5e4557a6-efa7-471a-85d0-7c45eda82307)


create database human_friends
use human_friends
DROP table if exists bankaccounts;

create TABLE bankaccounts (
    accountno varchar(20) PRIMARY KEY NOT NULL,
    funds decimal(8,2)
);

INSERT INTO bankaccounts VALUES('ACC1', 1000);
INSERT INTO bankaccounts VALUES('ACC2', 1000);


START TRANSACTION; -- statement1
UPDATE bankaccounts SET funds=funds-100 WHERE accountno='ACC1'; -- statement2
UPDATE bankaccounts SET funds=funds+100 WHERE accountno='ACC2'; -- statement3; 
commit;-- statement4

select * from bankaccounts
