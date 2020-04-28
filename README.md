# test_docker

## docker build guide
- docker build --rm -t one7ime/ubuntu_test .
- docker run -it --name test1 one7ime/ubuntu_test

## docker usage
```
root@6299c3e94601:/# tree |head
.
|-- bin -> usr/bin
|-- boot
|-- dev
|   |-- console
|   |-- core -> /proc/kcore
|   |-- fd -> /proc/self/fd
|   |-- full
|   |-- mqueue
|   |-- null


root@6299c3e94601:/home# ifconfig -a
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 172.17.0.2  netmask 255.255.0.0  broadcast 172.17.255.255
        ether 02:42:ac:11:00:02  txqueuelen 0  (Ethernet)
        RX packets 15  bytes 1186 (1.1 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        
root@6299c3e94601:/home# curl
curl: try 'curl --help' or 'curl --manual' for more information
root@6299c3e94601:/home# curl http://localhost
curl: (7) Failed to connect to localhost port 80: Connection refused
root@6299c3e94601:/home# curl http://google.com
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>301 Moved</TITLE></HEAD><BODY>
<H1>301 Moved</H1>
The document has moved
<A HREF="http://www.google.com/">here</A>.
</BODY></HTML>


```
