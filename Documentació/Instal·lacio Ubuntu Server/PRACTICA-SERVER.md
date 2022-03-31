1.Mostra el fitxer de configuració de la xarxa
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-25%2019-01-31.png)

2.Consulta l'adreça, màscara, porta d'enllaç i servidor DNS.
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-25%2019-42-53.png)
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-25%2019-39-57.png)

3.Canvia la configuració de Virtualbox  mode pont.
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-31%2015-27-26.png)

4.Renovar adreça i consultar
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-25%2019-45-17.png)

5.Posa una adreça manual, de la mateixa xarxa que l'Ubuntu Desktop de l'apartat anterior.
![](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Instal%C2%B7lacio%20Ubuntu%20Server/Imatges/Screenshot%20from%202022-03-25%2019-57-49.png)

6.Per a poder gestionar el servidor  remotament des de qualsevol terminal comprovarem si el servei SSH està actiu:
```console
  sudo service ssh status
  sudo systemctl status ssh
  ```
  
  >Si veiem active (running) ressaltat en verd vol dir que ja està instal·lat i funcionant. En cas que no, l'instal·larem:
 
```console
  sudo apt install openssh-server
  ```
  
7.Per a accedir al servei SSH:
  ssh usuari@adreça_IP

  Des d'on haurem de realitzar l'accés?
