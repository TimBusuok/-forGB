mkdir Work
cd ~/Work
cat > home_animals
cat > silly_animals
cat home_animals silly_animals > animals
cat animals
mv animals mans_friends
cd mans_friends
ll
cd ~
mkdir work_system
cd ~/Work
mv mans_friends ~/work_system
cd ~/work_system
ll
sudo wget https://dev.mysql.com/get/mysql-apt-config_0.8.23-1_all.deb
sudo dpkg -i mysql-apt-config_0.8.23-1_all.deb
sudo apt-get update
sudo apt-get install mysql-server
sudo wget https://download.docker.com/linux/ubuntu/dists/jammy/pool/stable/amd64/docker-ce-cli_20.10.13~3-0~ubuntu-jammy_amd64.deb
sudo dpkg -i docker-ce-cli_20.10.133-0ubuntu-jammy_amd64.deb
sudo dpkg -r docker-ce-cli
