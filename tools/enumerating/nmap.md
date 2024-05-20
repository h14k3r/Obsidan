## enumeration

#### flags

1. `-p-` --> scans all the TCP ports from 0-65535
2. `-sV` --> trys to determine the version of the service running on a port
3. `--min-rate` --> min number of packets nmap should send per second - scan speeds up as the number goes higher

> nmap -p- --min-rate 1000 -sV {IP}






