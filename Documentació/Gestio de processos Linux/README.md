## Gestió de processos Linux

1.Què és el PID d'un procés?
>Nombre identificador del proces.

2.Quina diferència hi ha entre l'opció -a i l'opció -x de l'ordre ps?
>Opció a mostra procés iniciats per l’usuari, mentre que la x mostra processos que pertanyen a l’usuari.

3.Què és el numero NICE d'un procés? Quins valors pot tenir? Quins usuaris el poden canviar?
>És la modificació de la prioritat, permet modificar des de -20 fins a 19, i només ho pot fer l’usuari root.

4.Utilitzant la comanda find. Busca tots els fitxers en el disc que comencin que tinguin l'extensió .h. Mentre s'executa la comanda mira en quina prioritat ho està fent?
```console
 find / -type f -iname "*h*"
 ps -lax
 ```
 5.Executa de nou la comanda anterior però aquest cop amb una prioritat mes baixa que la que te per defecte.
 ```console
 nice -n-10 find / -type f -iname "*h*"
 ```
 6.Obre un altre terminal i mentre l'ordre anterior s'executa, mitjançant la comanda ps llista tots els processos associats al terminar de l'usuari actual i obté el PID del procés ls. 
 ```console
 ps -e
  ```
 7.Amb l'ordre renice atorga la màxima prioritat a l'ordre ls anterior.
 ```console
 renice -n-20 ls
 ```
 8.Ara amb l'ordre kill finalitza el procés.
```console
kill 11123
 ```
 9.Visualitza mitjançant l'editor nano l'arxiu que conté la informació dels usuaris del sistema.
 ```console
 nano etc/passwd
 nano etc/shadow
 ```
 10.En una altra terminal, obté el PID de l'editor i el PID del seu procés pare mitjançant la comanda pstree.
 ```console
 pstree -g
 ```
 [Captura Pantalla pstree -g del PID nano i el seu parent](
