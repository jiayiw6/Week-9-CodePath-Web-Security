# Week-9-CodePath-Web-Security

1. Which Honeypot(s) you deployed
mhn-honeypot-1	35.239.51.107   dionaea

2. Any issues you encountered
VM in GCloud does not allow HTTP and HTTPS requests by default, user will need to go to instance -> edit -> allow HTTP/HTTPS to access the MHN admin console. This was not stated in the instruction and was casuing some confusions. 

3. A summary of the data collected: number of attacks, number of malware samples, etc.
3137 attacks in ~10 minutes after deloyment. 
Most popular Protocol: pcap
Most popular Dst Port: 8080

4. Any unresolved questions raised by the data collected
As the instruction stated, 3 open ports should be shown. 
Well, I have a little bit more than 3 ports open.. 

Nmap scan report for 107.51.239.35.bc.googleusercontent.com (35.239.51.107)  
Host is up (1.2s latency).  
Not shown: 987 closed ports  
PORT     STATE    SERVICE  
21/tcp   open     ftp  
22/tcp   open     ssh  
25/tcp   filtered smtp  
42/tcp   open     nameserver  
80/tcp   open     http  
135/tcp  filtered msrpc  
139/tcp  filtered netbios-ssn  
443/tcp  open     https  
445/tcp  filtered microsoft-ds  
1433/tcp open     ms-sql-s  
3306/tcp open     mysql  
5060/tcp open     sip  
5061/tcp open     sip-tls  

5.Additionally, include a json export of the data you collected in the repo.
https://raw.githubusercontent.com/jiayiw6/Week-9-CodePath-Web-Security/master/session.json
