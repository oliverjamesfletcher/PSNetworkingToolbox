# PSNetworkingToolbox

Run networking commands from a PowerShell console menu

This script allows you to select a networking command then set variables and run.

## Install Instructions

1. Download ZIP [here](https://github.com/oliverjamesfletcher/PSNetworkingToolbox/blob/master/License)
2. Create folder in the root of C:\ named "Scripts"
3. Extract files into "Scripts" folder

## Usage

1. Run PS and cd to C:\Scripts
2. Enter .\Networking_Toolbox.ps1 and press enter to run toolbox

######Note: Some commands will display information, others will require input

## Commands Included

####1. Ipconfig

Displays all current TCP/IP network configuration values and refreshes Dynamic Host Configuration Protocol (DHCP) and Domain Name System (DNS) settings. Used without parameters, ipconfig displays the IP address, subnet mask, and default gateway for all adapters.

####2. Ipconfig /all

Displays the full TCP/IP configuration for all adapters. Without this parameter, ipconfig displays only the IP address, subnet mask, and default gateway values for each adapter. Adapters can represent physical interfaces, such as installed network adapters, or logical interfaces, such as dial-up connections.

####3. Netstat

Displays active TCP connections, ports on which the computer is listening, Ethernet statistics, the IP routing table, IPv4 statistics (for the IP, ICMP, TCP, and UDP protocols), and IPv6 statistics (for the IPv6, ICMPv6, TCP over IPv6, and UDP over IPv6 protocols). Used without parameters, netstat displays active TCP connections.

####4. Netstat -a

Displays all active TCP connections and the TCP and UDP ports on which the computer is listening.

####5. Nslookup

Displays information that you can use to diagnose Domain Name System (DNS) infrastructure. Before using this tool, you should be familiar with how DNS works. The Nslookup command-line tool is available only if you have installed the TCP/IP protocol.

####6. Tracert

Determines the path taken to a destination by sending Internet Control Message Protocol (ICMP) Echo Request or ICMPv6 messages to the destination with incrementally increasing Time to Live (TTL) field values. The path displayed is the list of near/side router interfaces of the routers in the path between a source host and a destination. The near/side interface is the interface of the router that is closest to the sending host in the path. Used without parameters, tracert displays help.

####7. Pathping 

Provides information about network latency and network loss at intermediate hops between a source and destination. Pathping sends multiple Echo Request messages to each router between a source and destination over a period of time and then computes results based on the packets returned from each router. Because pathping displays the degree of packet loss at any given router or link, you can determine which routers or subnets might be having network problems. Pathping performs the equivalent of the tracert command by identifying which routers are on the path. It then sends pings periodically to all of the routers over a specified time period and computes statistics based on the number returned from each.

####8. Netsh int ip reset all 

Reset all NIC TCP/IP

######Warning: This will remove all static ip addreses set

####9. Ping

Verifies IP-level connectivity to another TCP/IP computer by sending Internet Control Message Protocol (ICMP) Echo Request messages. The receipt of corresponding Echo Reply messages are displayed, along with round-trip times. Ping is the primary TCP/IP command used to troubleshoot connectivity, reachability, and name resolution.

####10. Ping -t

Specifies that ping continue sending Echo Request messages to the destination until interrupted. To interrupt and display statistics, press CTRL-BREAK. To interrupt and quit ping, press CTRL-C.

####11. Telnet "port number"

Check if a certain port is open on a remote host

####12. Getmac

Returns the media access control (MAC) address and list of network protocols associated with each address for all network cards in each computer.

####13. Arp

Displays entries in the Address Resolution Protocol (ARP) cache, which contains one or more tables that are used to store IP addresses and their resolved Ethernet or Token Ring physical addresses.

####14. Hostname

Displays the host name portion of the full computer name of the computer and the domain it is connected to.

####15. Route add

Add a route with variables set (Destination, Subnet Mask and Gateway) to the IP routing table

####16. Route add if

Add route with variables set (NIC Index, Destination, Subnet Mask and Gateway) to the IP routing table

####17. Route add if metric

Add a route with variables set (NIC Index, Destination, Subnet Mask and Gateway) to the IP routing table

####18. Route -p add

Add a persistent route with variables set (Destination, Subnet Mask and Gateway) to the IP routing table

####19. Route -p add if

Add a persistent route with variables set (NIC Index, Destination, Subnet Mask and Gateway) to the IP routing table

####20. Route delete

Remove route and variables set (Destination, Subnet Mask and Gateway) from the IP routing table

##License

The license is available [here](https://github.com/oliverjamesfletcher/PSNetworkingToolbox/blob/master/License)
