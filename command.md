# [HackLabsBook]


## Enumeración sitios web
 **GoBuster**
 {Kali Linux} gobuster dir -u http://10.10.10.171 -w /usr/share/wordlists/dirbuster/directory-list-2.3-small.txt [enter] >> Se muestran los directorios que existen en el sitio web a partir de la búsqueda de diccionario.
 
 **Nikto**
 {Kali Linux} nikto -h 192.168. 0.70 -p 80 >> Permite escanear vulnerabilidades en un sitio web -h Corresponde a la ip o nombre de host -p Corresponde al puerto donde está expuesto el sitio web

## Escaneo de puertos 
**Nmap básico**
- nmap -sC -sS -Pn -T5 -p T:1-65535,U:1-65535 192.168.0.17 >> scan
- Nmap –sV –Pn  -T5 172.18.1.48 >> scan
	
**Nmap con script**
- nmap -p 80 --script=http-backup-finder --script-args http-backup-finder.url=/web-serveur/ch11/index.php challenge01.root-me.org >> Busca un archivo en la URL con la palabra "backup"


## Hash
 {Kali Linux} Hash-identifier [enter] luego se ingresa el hash que queremos investigar


## Tunneling

**Tunel mediante OpenSSH**
{Kali Linux} ssh -L 443:127.0.0.1:443 user@10.10.10.184 >> ssh -L (puerto-local-escucha):(host-remoto):(puerto-remoto) (servidor-ssh)


## Comandos básicos Hack Linux

- sudo -l -n >> Indica las ubicaciones dónde el usuario autenticado tiene permisos como root
