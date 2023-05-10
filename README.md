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
# Ping test
ping will happen between:
ubuntu2 to ovs and vice versa
ubuntu3 to ovs and vice versa

ping will not happen between:
ubuntu2 and ubuntu3 and vice versa

# Adding a bridge in OVS
This will allow the trafic to flow between the two instances ubunt2 and ubuntu3
```
ovs-vsctl add-br br0
ovs-vsctl br0 up
ovs-vsctl show
ovs-vsctl add-port br0 eth0
ovs-vsctl add-port br0 eth1
ovs-vsctl show

```

