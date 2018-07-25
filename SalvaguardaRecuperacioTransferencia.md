Salvaguarda. Recuperació. Transferència
===================

Concepte de seguretat i recuperació
---------------------
En termes informàtics i, més concretament, pel que fa a les bases de dades, a **tenir cura de les dades** duent-ne a terme una o diverses còpies de seguretat, o bé duent a terme les accions necessàries per mantenir les dades protegides davant possibles accessos no desitjables o altres atacs.

La **recuperació de les dades** defineix el procediment mitjançant el qual s'accedirà a la base de dades per recuperar la versió estable de la base de dades emmagatzemada com a còpia de seguretat i poder recuperar o arribar a substituir, d'aquesta manera, la base de dades operativa.

Seguretat
---------------------
Els aspectes més importants per a la seguretat són la planificació dels processos que executaran la seguretat (els paràmetres que cal tenir en compte, com, quan…), l'estudi dels tipus de suports existents (RAI, servidors, duplicats…) i dels tipus de còpies de seguretat que hi ha, com, per exemple, les còpies incrementals, les còpies acumulatives o les còpies de seguretat completes.

###  Planificació

Tot projecte de desenvolupament d'una aplicació informàtica requereix, en la fase de disseny, el desenvolupament d'un pla de contingència que prevegi una política de còpies de seguretat.


El pla de seguretat i tota la infraestructura que envolta la informació és un dels pilars bàsics que sustenten l'èxit o el fracàs d'una organització, i s'arriba a externalitzar aquest servei contractant proveïdors de seguretat, encarregats de la seguretat de la informació confidencial que es manipula a l'organització.

L'RLOPD estableix la còpia de seguretat en un fitxer automatitzat sobre un suport que en permeti la recuperació. La llei obliga a documentar els procediments en què quedin descrites les accions de còpies de seguretat i les accions de restauració o recuperació d'aquestes dades. Aquests procediments podran ser revisats per auditories per garantir-ne la qualitat. De fet, l'RLOPD obliga que, cada sis mesos, el responsable dels fitxers verifiqui la definició, el funcionament i l'aplicació correctes dels processos de còpies de seguretat i de recuperació de dades.

### Tipus de suports

Una vegada s'ha planificat el procés de seguretat, el responsable del desenvolupament d'un programari o el responsable del sistema informàtic han de determinar quina és la millor opció, entre els suports existents en el mercat, per emmagatzemar les dades que faran servir durant l'execució. Però haurà de tenir en compte, per als suports físics, el sistema en producció, un possible sistema de desenvolupament o proves i un sistema de còpies de seguretat.

La **replicació de les dades** consisteix a copiar les dades d'una ubicació física a una altra, normalment per blocs i de manera diferencial. Les dades que han canviat a la font o al sistema en producció queden replicades de manera automàtica en el sistema de seguretat o de destinació.

En els sistemes que fan servir la tècnica de la replicació de dades caldrà arribar al compromís entre estar sempre actualitzat però afectar el rendiment del sistema origen, o bé no afectar-ne el rendiment, però córrer el risc de desincronitzar-se molt ràpidament.

###  Tipus de còpies de seguretat

Les còpies de seguretat es poden dur a terme de moltes maneres, ja que hi ha molts tipus diferents de còpies de seguretat. Caldrà escollir les més adients en cada cas, en funció de l'aplicació o aplicacions informàtiques o del tipus de sistema informàtic que es faci servir.

Les còpies completes, com el seu nom indica, duran a terme una còpia de tot el que hi ha en el sistema d'origen. Són un tipus de còpia sense gaires secrets. Es tracta de copiar tot el que es troba en el sistema d'origen (ja siguin totes les dades o totes les dades i totes les aplicacions) i emmagatzema en el sistema de destinació. El problema és l'espai. En el cas de tenir una gran quantitat de dades caldrà disposar d'un sistema de destinació o de seguretat que sigui, com a mínim, igual de gran que el sistema d'origen.

Les còpies parcials són les que, com el seu nom indica, no duran a terme una còpia completa de tot el sistema o de tots els arxius de dades, sinó que copiarà només una part determinada dels arxius o del sistema. Aquests tipus de còpies, les còpies parcials, només copiaran els arxius que s'hagin modificat des de la darrera vegada que s'hagi dut a terme un procediment de seguretat, sense tornar a copiar tots els arxius que siguin iguals en el sistema d'origen i en el sistema de destinació.

Les còpies parcials poden ser incrementals o diferencials.
* Les **còpies incrementals** són aquelles en què només es copiaran els
fitxers modificats o creats des de la darrera còpia incremental feta.
* Les **còpies diferencials** són aquelles en què només es copiaran els
fitxers modificats o creats des de la darrera còpia completa.

Recuperació de les dades
---------------------

Una vegada s'ha assegurat la informació de manera automàtica o ho han fet els responsables d'executar aquests procediments, podrà ser necessària la recuperació parcial o total d'aquesta informació.

Per entendre correctament els sistemes de recuperació de dades caldrà revisar les diferents propostes de tipus de còpies de seguretat que es podran utilitzar. Serà diferent dur a terme uns procediments de recuperació de les dades assegurades de manera completa o de manera parcial, de les dades guardades encriptades, de les guardades sense encriptar o de les que es trobin en un sistema de rotació diari i de les que ho facin de manera setmanal.

Les còpies completes permeten la restauració d'un sistema de manera molt senzilla davant una catàstrofe. Per aquesta raó, és important dur a terme una còpia de seguretat completa de tot el sistema informàtic de manera periòdica per preveure aquesta casuística.

Utilitats per a la seguretat i recuperació
---------------------
Una bona selecció d'una aplicació per fer i recuperar còpies de seguretat dependrà de les necessitats que es tinguin, la ubicació física (tipus i lloc) de les dades i del sistema informàtic on es duran a terme.

Sentències per fer i recuperar còpies de seguretat
---------------------


Hi ha algunes sentències dels llenguatges de programació de quarta generació que incorporen sentències SQL que permeten la realització i la recuperació de còpies de seguretat tant de les estructures i de les característiques de les bases de dades com de les dades que contenen.

Les sentències SQL que permeten dur a terme aquestes accions són:

* **Backup**, que permet crear una còpia de seguretat d'una base de dades. Aquesta sentència permet treballar tant amb els fitxers que contenen la definició de les taules com amb els fitxers que contenen les dades.
* **Restore**, que permet la restauració a partir d'una còpia de seguretat d'una taula de la base de dades, en què s'hagi fet servir la sentència Backup. La restauració podrà ser de tota la base de dades, d'una part o la restauració de la base de dades en un punt concret en què s'hagi fet una captura de la situació.





Transferència de dades
---------------------

La transferència de dades serà necessària quan s'ha d'establir una comunicació entre diferents bases de dades, ja sigui que utilitzin el mateix sistema gestor de bases de dades o diferents.

###  Utilitats per importar i exportar dades

La importació de dades consisteix a fer una càrrega d'informació, de dades, a una base de dades ja existent, amb la seva estructura ja creada. Aquesta importació permet automatitzar la càrrega de dades de la base de dades a partir d'informacions tractades amb altres sistemes (bloc de notes, arxius de fulls de càlcul…) o amb altres aplicacions.

###  Interconnexió i migració de dades entre diferents SGBD

La transferència de bases de dades, o d'una part, es podrà dur a terme entre dos sistemes que facin servir el mateix sistema gestor de bases de dades a partir d'aplicacions o de sentències pròpies.
