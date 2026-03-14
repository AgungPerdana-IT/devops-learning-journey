# Network Basics

1. `ip a` - Show network interfaces and IP address
2. `ip route` - Show routing table
3. `ping` - Test connectivity to other host
4. `curl ifconfig.me` - Get public IP address
5. `ss -tulnp` - Show open ports and services
6. `dig google.com` - Query DNS record
7. `nslookup google.com` - Similar to `dig google`
8. `traceroute google.com` - Show path packets take to reach a host


## Example Troubleshooting Workflow
### Example steps when internet is not working
1. Check IP address
    `ip a`
2. Check gateway
    `ip route`
3. Test Connectivity
    `ping 8.8.8.8`
4. Test DNS
    `dig google.com`
5. Check open ports
    `ss -tulnp`