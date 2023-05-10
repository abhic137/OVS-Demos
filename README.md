## OVS-Demos
#install docker and docker compose

```
sudo docker-compose up -d
sudo docker ps
```
# Inside Ubuntu2 Terminal
```
#in seperate terminal
sudo docker exec -it ubuntu2 bash
apt update
apt install net-tools
apt-get install iputils-ping
```
# Inside Ubuntu3 Terminal
```
#in seperate terminal
sudo docker exec -it ubuntu3 bash
apt update
apt install net-tools
apt-get install iputils-ping
```
# Inside OVS Terminal
```
#in seperate terminal
sudo docker exec -it ovs bash
apt update
apt install net-tools
apt-get install iputils-ping
```
