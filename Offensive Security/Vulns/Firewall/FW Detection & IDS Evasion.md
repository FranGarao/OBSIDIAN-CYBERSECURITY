nmap: 
	-sA (very useful)
     -f (fragmented packets for evasion :D)
     -mtu 32 (32=example)
     --ttl (time-to-live)
     -D 10.10.10.10.,ME,12.12.12.12, 19.43.222.34 (differents ips)
     --data-length 200
     -g 53 (change port)