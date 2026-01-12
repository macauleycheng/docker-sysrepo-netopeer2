# Dockerfile for sysrepo-netopeer2 setup

To run `sysrepod` and `netopeer2-server` use the command:
```
docker run -i -t --name sysrepo --rm sysrepo/sysrepo-netopeer2:latest
```
or via SSH to port `830` (username / password is `netconf`):
```
docker inspect sysrepo | grep -w "IPAddress"
# assuming output of the above commnd to be 172.17.0.3
ssh netconf@172.17.0.3 -p 830 -s netconf 
```
