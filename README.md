## OVS-Demos
## install docker and docker compose

sudo docker-compose up -d
sudo docker ps

#in seperate terminal
sudo docker exec -it ubuntu2 bash
apt update
apt install net-tools
apt-get install iputils-ping

#in seperate terminal
sudo docker exec -it ubuntu3 bash
apt update
apt install net-tools
apt-get install iputils-ping

#in seperate terminal
sudo docker exec -it ovs bash
apt update
apt install net-tools
apt-get install iputils-ping
