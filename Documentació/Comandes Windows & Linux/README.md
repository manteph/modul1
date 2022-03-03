| ![](RackMultipart20220303-4-1ve1fn3_html_aec8a7489275c163.png) | **GESTIÓ DE FITXERS I DIRECTORIS EN LINUX** |
| --- | --- |

**1**. **(0,5 punts)** Crea la següent estructura de subdirectoris en el teu HOME:

![](RackMultipart20220303-4-1ve1fn3_html_2a0d6772c5e881.png)

| **COMANDES:**![](RackMultipart20220303-4-1ve1fn3_html_4368b46cdc3b7690.png)


 |
| --- |

**2.**** (0,5 punts) **Crea un arxiu dins de la carpeta** C **que s&#39;anomeni** programa.c **i crea un arxiu dins de la carpeta** JAVA **que s&#39;anomeni** programa.java**.

| **COMANDES:**** t ![](RackMultipart20220303-4-1ve1fn3_html_daf0bc63364925b0.png) ouch programa.java** |
| --- |

**3.**** (0,5 punts) **Crea un arxiu dins de la carpeta** HARD **que s&#39;anomeni** apunts.hard **i crea un arxiu dins de la carpeta** SOFT **que s&#39;anomeni** apunts.soft**.

| **COMANDES:touch apunts.hard**** touch apunts.soft**
 |
| --- |

**4.**** (0,5 punts)** Configureu els següents permisos d&#39;accés al vostre arbre de directoris C2 de tal forma que els usuaris del sistema que pertanyen al vostre grup podran accedir al vostre directori només per llegir els documents. La resta d&#39;usuaris no tindran cap tipus d&#39;accés.

| **COMANDES** :chmod g-wx c2chmod o-rwx c2
 |
| --- |

**5.**** (0,5 punts) **Els usuaris del vostre grup podran accedir a l&#39;estructura de directoris que heu creat, però no podran accedir a les carpetes** HARD **i** C**, perquè teniu arxius que no voleu que els puguin llegir.

| **COMANDES:**** chmod g-rwx c2/treballs/hard ****chmod g-rwx c8/programes/c** |
| --- |

**6**. **(0,5 punts)** En una única sentència fes una llista completa de tots els arxius del directori **/etc** que comencin per **s**.

Posa una **X** a la columna **SI** , si la sentència és correcta i explica que fa.

Posa una **X** a la columna **NO** , si la sentència no és correcta i explica perquè no ho és.

**7.**** (0,5 punts) ls -la \&gt; usuaris**

| **SI** | **NO** | **Explicació** |
| --- | --- | --- |
| **x** |
 | Crea archiu amb la surtida del comando ls -la |

**8**. **(0,5 punts) wc -l usuaris**

| **SI** | **NO** | **Explicació** |
| --- | --- | --- |
| **x** |
 | Conta les linies del fitxer usuaris |

**9. (0,5 punts) rm usuaris**

| **SI** | **NO** | **Explicació** |
| --- | --- | --- |
| **x** |
 | Elimina el fitxer usuaris |

**10.**** (0,5 punts)** Què poden fer els diferents usuaris de Linux amb un arxiu que té els següents permisos:

**-r- xr- ----**

| Res, ja que ni poden veure el fitxer
 |
| --- |

**11. (0,5 punts)** Canvia els permisos de l&#39;arxiu per tal que el propietari pugui modificar l&#39;arxiu, el seu grup puguin llegir-lo i executar-lo i la resta d&#39;usuaris només llegir-lo.

| **COMANDA: chmod +w, g-w, o-wx**** chmod 254**
 |
| --- |

**12**. **(0,5 punts)** Escriu la seqüència de comandes necessàries per a crear el directori **EXERCICI13 dins del directori EXERCICIS.**

| **COMANDA:mkdir** _ **home/c2/exercicis/exercici13** _


 |
| --- |

**13.**** (0,5 punts) **Dins del directori EXERCICI13 crea el directori** PROVA **i copia a dins de PROVA l&#39;arxiu** /etc/passwd.**

| **COMANDES:**** cp passwd /home/gheorghe/Documents/&quot;curs programacio de sistemes&quot;/c2/exercicis/exercici13/prova**
 |
| --- |

**14.**** (0,5 punts)** Com ho faries sense moure&#39;t del directori arrel si et trobes dins del directori SOFT.

| **COMANDA:cp /etc/passwd /home/gheorghe/Documents/&quot;curs programacio de sistemes&quot;/c2/exercicis/exercici13/prova**


 |
| --- |

**15.**** (0,5 punts)**Quina sentencia utilitzaries si et trobes en el directori arrel (/) i vols moure un arxiu COTXES.txt ubicat a**/home/prova **al directori** /etc**

| **COMANDA:mv** _ **home/** _ **prova/cotxes.txt /etc**  **també serveis per canviar nom d&#39;un arxiu**
 |
| --- |

**16**. **(0,5 punts)** Et trobes en el teu directori **HOME** i vols esborrar tot el seu contingut, inclosos els subdirectoris que conté. Com ho faries amb una única sentència?

| **COMANDA:**
 |
| --- |

**17**. **(0,5 punts)** En una única sentència fes que: (cal utilitzar **|** per separar comandes)

- Es visualitzi per pantalla un arxiu de text.
- Guarda el resultat en un arxiu anomenat **resultat**.

| **COMANDA:**
 |
| --- |

**18**. **(0,5 punts)** En una única sentència d&#39;ordres realitza les accions oportunes per tal que el mes actual es quedi emmagatzemat en un arxiu anomenat **mes\_actual**.

| **COMANDA:**
 |
| --- |

**19.**** (0,5 punts) **Busca amb la comanda** find** on està ubicat l&#39;arxiu COTXES.txt

| **COMANDA:**
 |
| --- |

**20. (0,5 punts)** Busca amb la comanda **find** tots els arxius de l&#39;equip que superin els 2000Kb de tamany.

| **COMANDA:**
 |
| --- |
