baseUrl: https://api.hospitaldeclinicas.uba.ar
port: ==443==
service: ==Apache/2.4.56 (Debian)==

|_ssl-date: TLS randomness does not represent time
|_http-cors: ==HEAD GET POST PUT DELETE PATCH==
| ssl-cert: Subject: ==commonName=api.hospitaldeclinicas.uba.ar==
| Subject Alternative Name: DNS:api.hospitaldeclinicas.uba.ar
| Not valid before: ==2024-09-30T12:05:06==
|_Not valid after:  ==2024-12-29T12:05:05==
|_http-title: ==Google Signin==
MAC Address: ==00:0C:29:BD:FD:8A (VMware)== 

IPs ==10.10.18.228, 157.92.188.14
+ Target IP:          ==10.10.18.228==
+ Target Hostname:    api.hospitaldeclinicas.uba.ar
+ Target Port:        443
---------------------------------------------------------------------------
+ SSL Info:        Subject:  /CN=api.hospitaldeclinicas.uba.ar
                   Ciphers:  TLS_AES_256_GCM_SHA384
                   Issuer:   /C=US/O=Let's Encrypt/CN=E6
+ Start Time:         2024-10-22 10:32:30 (GMT-4)
---------------------------------------------------------------------------
+ Server: Apache/2.4.56 (Debian)
+ /: Retrieved x-powered-by header: Express.
+ /: Retrieved access-control-allow-origin header: *.
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The site uses TLS and the Strict-Transport-Security HTTP header is not defined. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ /: Cookie ROUTEID created without the secure flag. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies
+ /: Cookie ROUTEID created without the httponly flag. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ /: Server may leak inodes via ETags, header found with file /, inode: W/255, size: 18e2dea02f4, mtime: gzip. See: http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2003-1418
+ /: The Content-Encoding header is set to "deflate" which may mean that the server is vulnerable to the BREACH attack. See: http://breachattack.com/
+ 8130 requests: 0 error(s) and 9 item(s) reported on remote host
+ End Time:           2024-10-22 10:35:55 (GMT-4) (205 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
