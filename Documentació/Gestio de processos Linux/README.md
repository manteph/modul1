## Gestió de processos Linux

### Respon les següents preguntes

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
 ![Captura Pantalla pstree -g del PID nano i el seu parent](https://github.com/manteph/modul1/blob/main/Documentaci%C3%B3/Gestio%20de%20processos%20Linux/Screenshot%20from%202022-03-11%2017-52-03.png)

### Processos en primer pla

1.Quina comanda utilitzaries per mira els processos existents al sistema. 
```console
ps -aux
```
2.Llença un procés que duri 600 segons en primer pla. (per exemple  sleep 600).
```console
sleep 600
```
3.Mata el procés anterior. Que observes? Apareixen els mateixos processos que al punt 1?
```console
kill 12554
ps -aux
```
>Havent matat el procés hi surten els mateixos que al punt 1.
4.Torna a executar el procés però ara pararem el procés (Control-Z) Que observes? Apareixen els mateixos processos que al punt 1?
>No, ja que para el procés, només el posa en pausa no el mata, per lo que aquest hi continua surtint com procés iniciat.
5.Mata finalment el procés.
```console
kill 13231
```
### Processos en segon pla

1.Executa un procés qualsevol en segon pla.
```console
firefox </dev/null &>/dev/null &
```
2.Un procés en segon pla, seguirà mostrant la seva sortida per pantalla des de que s'ha donat l'ordre d'execució?
>Al passar-lo en segon pla, ja no mostra les sortides en terminal.
3.Para el procés.
```console
firefox
^Z
```
4.Reinicia el procés anterior i que aquest segueixi en segon pla.
```console
jobs
fg firefox
```
