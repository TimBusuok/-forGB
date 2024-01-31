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
