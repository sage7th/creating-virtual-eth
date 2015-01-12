# creating-virtual-eth
#ip link add eth0 type veth peer name=eth0-port
# ip tuntap add dev eth0 mode tap
# ip link ls dev eth0
 eth0: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN mode DEFAULT qlen 500
    link/ether 0e:55:9b:6f:57:6c brd ff:ff:ff:ff:ff:ff
# tunctl -t eth0
Set 'eth0' persistent and owned by uid 0
# ifconfig eth0
eth0      Link encap:Ethernet  HWaddr a6:9b:fe:d8:d9:5e  
          BROADCAST MULTICAST  MTU:1500  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:500 
          RX bytes:0 (0.0 B)  TX bytes:0 (0.0 B)
