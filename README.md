# docker-alpine-tinyproxy
dockerfile for tinyproxy on alpine linux.

# proxy port
port is ```8888```.

# how to use
docker run -d -p 8888:8888 sinfseven/alpine-tinyproxy

# my setting
This content is written in tinyproxy.conf.  
(tinyproxy.conf is a partial rewrite of the default configuration file)  

- ```(default)``` -> ```(mine)```
- ```MinSpareServers 5``` -> ```MinSpareServers 20```
- ```MaxSpareServers 20``` -> ```MaxSpareServers 60```
- ```StartServers 10``` -> ```StartServers 25```
- ```MaxRequestsPerChild 0``` -> ```MaxRequestsPerChild 10000```
- ```Allow 127.0.0.1``` -> ```#Allow 127.0.0.1```
- ```ViaProxyName "tinyproxy"``` -> ```#ViaProxyName "tinyproxy"```
