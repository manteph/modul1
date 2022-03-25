1.Mostra el fitxer de configuració de la xarxa
2.Consulta l'adreça, màscara, porta d'enllaç i servidor DNS.
3.Canvia la configuració de Virtualbox  mode pont.
4.Renovar adreça i consultar
5.Posa una adreça manual, de la mateixa xarxa que l'Ubuntu Desktop de l'apartat anterior.
6.Per a poder gestionar el servidor  remotament des de qualsevol terminal comprovarem si el servei SSH està actiu:
  sudo service ssh status
  sudo systemctl status ssh
  Si veiem active (running) ressaltat en verd vol dir que ja està instal·lat i funcionant. En cas que no, l'instal·larem:

  sudo apt install openssh-server
7.Per a accedir al servei SSH:
  ssh usuari@adreça_IP

  Des d'on haurem de realitzar l'accés?
