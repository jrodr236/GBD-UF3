Salvaguarda. Recuperació. Transferència
===================

[Veure teoria](https://jrodr236.github.io/GBD-UF3/SalvaguardaRecuperacioTransferencia)

---

Concepte de seguretat i recuperació
---------------------
**Tenir cura de les dades**: còpies de seguretat o dur accions per protegir d'accessos no desitjables o altres atacs.

**Recuperació de les dades**: recuperar la còpia de seguretat.

---

Seguretat
---------------------

* Planificació de processos
* Tipus de suports
* Tipus de còpies de seguretat

+++

###  Planificació

Pla de contingència:

**Què** emmagatzemar?

**Quan** fer-ho?

**On** desar les dades?

**Com**, tipus de suport?

Com fer **restauració**?

+++

### Tipus de suports

Discos durs

Discos compactes

Cintes magnètiques

Discos durs externs

Unitats Flash o memòries USB

SAN

RAID

+++

**Replicació de les dades**: copiar les dades d'una ubicació física a una altra.

Compromís:
* estar sempre actualitzat però afectar el rendiment del sistema origen
* no afectar-ne el rendiment, però córrer el risc de desincronitzar-se molt ràpidament

+++

###  Tipus de còpies de seguretat

* Completes
* Parcials
  * Incrementals: modificacions des de la última incremental
  * Diferencials: modificacions des de la última completa

+++

Incremental
![Còpia incremental](http://static.couchbaseinc.hosting.ca.onehippo.com/images/server/3.x/20170420-170703/backup-differential-incremental.jpg)

+++

Diferencial
![Còpia diferencial](http://static.couchbaseinc.hosting.ca.onehippo.com/images/server/3.x/20170420-170703/backup-cumulative-incremental.jpg)

+++

Combinació

![Combinació d'incremental i diferencial](http://static.couchbaseinc.hosting.ca.onehippo.com/images/server/3.x/20170420-170703/backup-combined-incremental.jpg)

---

Recuperació de les dades
---------------------

Parcial o total.

Dependrà de la còpia de seguretat: completa/parcial, encriptades o no, diàries/setmanals.

---

Utilitats per a la seguretat i recuperació
---------------------

Integrada en el SGBD / externa

---

Sentències per fer i recuperar còpies de seguretat
---------------------
```SQL
Backup
Restore
```

No funcionen a tots els SGBD.

---


Transferència de dades
---------------------

Comunicació entre diferents bases de dades, amb el mateix SGBD o diferent.

* Utilitats per importar i exportar dades
* Interconnexió i migració de dades entre diferents SGBD
