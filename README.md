# [HackLabsBook]

## PORT SCAN
** Escaneo inicial
nmap -sC -sS -Pn -T5 -p T:1-65535,U:1-65535 192.168.0.17 > scan
	
** Nmap con script 
nmap -p 80 --script=http-backup-finder --script-args http-backup-finder.url=/web-serveur/ch11/index.php challenge01.root-me.org
