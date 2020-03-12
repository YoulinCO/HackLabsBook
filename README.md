# [HackLabsBook]

## PORT SCAN
**Nmap básico**
- nmap -sC -sS -Pn -T5 -p T:1-65535,U:1-65535 192.168.0.17 > scan
- Nmap –sV –Pn  -T5 172.18.1.48 > scan
	
**Nmap con script**
- nmap -p 80 --script=http-backup-finder --script-args http-backup-finder.url=/web-serveur/ch11/index.php challenge01.root-me.org >> Busca un archivo en la URL

## HASH
 {Kali Linux} Hash-identifier [enter] luego se ingresa el hash que queremos investigar

## Comandos básicos Hack Linux

- sudo -l -n >> Indica las ubicaciones dónde el usuario autenticado tiene permisos como root
