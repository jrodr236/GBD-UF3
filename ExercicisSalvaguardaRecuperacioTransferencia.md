Salvaguarda. Recuperació. Transferència - Exercicis pràctics
===================

Pla de contingència
----------------------

Descarrega el següent pla de contingència: https://tavistockandportman.nhs.uk/documents/73/ict-failure-contingency-plan.pdf

Identifica els conceptes bàsics respecte a la seguretat de les bases de dades:
1. **Què**: quines parts o dades del projecte cal emmagatzemar.
1. **Quan**: quan s’haurà de dur a terme el procés de seguretat i cada quan s’haurà
de repetir.
1. **On**: on s’hauran de guardar aquestes dades, establint-ne la ubicació física.
1. **Com**: en quin tipus de suport s’han d’emmagatzemar les còpies de seguretat.
1. Com s’haurà d'actuar per
dur a terme la **restauració** de les dades assegurades en el cas eventual de
necessitat de recuperar el sistema de còpies de seguretat *(backups)* o accedir-
hi.

En cas que algun dels conceptes no quedi clar o no s'especifiqui, indica-ho i fes una proposta per resoldre-ho.


Transferència de dades
-------------------------
> Per a realitzar aquesta pràctica has d'escollir dos SGBD relacionals, els que vulguis: My_SQL/MariaDB, PostgreSQL, Oracle Database, Microsoft SQL Server, ~~MongoDB~~, etc...
> Es recomana descarregar dues *Virtual Appliance*, per exemple de [bitnami](https://bitnami.com/stacks/database), per estalviar-te el desplegament.

1. Descarrega alguna base de dades d'exemple amb un volum de dades una mica alt. Per exemple [aquesta per MySQL](http://downloads.mysql.com/docs/world.sql.gz).
1. Crea una nova base de dades amb la informació descarregada a un dels SGBD.
1. Fes algun canvi a la base de dades.
1. Transfereix la base de dades creada, incloent les modificacions que has fet, a l'altre SGBD.

> No és vàl·lid importar la base de dades descarregada a l'altre SGBD i després repetir les modificacions fetes, cal utilitzar algunes eines que permetin importar+exportar o fer la transferència directament.


Copies de seguretat i restauració
-------------------------------
> Per a realitzar aquesta pràctica pots escollir l'SGBD que vulguis: My_SQL/MariaDB, PostgreSQL, Oracle Database, Microsoft SQL Server, MongoDB, etc...
> Es recomana descarregar una *Virtual Appliance*, per exemple de [bitnami](https://bitnami.com/stacks/database), per estalviar-te el desplegament.

### Creació de la Base de Dades

1. Descarrega alguna base de dades d'exemple amb un volum de dades una mica alt. Per exemple [aquesta per MySQL](http://downloads.mysql.com/docs/world.sql.gz).
1. Crea una nova base de dades amb la informació descarregada.

### Còpia total

1. Fes una còpia de seguretat *completa* de la base de dades.
1. Simula un *crash* de l'SGBD.
1. Restaura la còpia de seguretat.
1. Verifica que s'han recuperat les dades correctament.

### Còpia diferencial

1. Fes una còpia de seguretat *completa* de la base de dades, si cal, o recupera l'anterior.
1. Modifica alguna dada de la base de dades.
1. Fes una còpia *diferencial*.
1. Modifica alguna altra dada de la base de dades.
1. Fes una altra còpia *diferencial*.
1. Respon: quines de les còpies fetes caldran per fer una restauració?
1. Simula un *crash* de l'SGBD.
1. Restaura les còpies de seguretat necessàries.
1. Verifica que s'han recuperat les dades correctament.

### Còpia incremental

1. Fes una còpia de seguretat *completa* de la base de dades, si cal, o recupera l'anterior.
1. Modifica alguna dada de la base de dades.
1. Fes una còpia *incremental*.
1. Modifica alguna altra dada de la base de dades.
1. Fes una altra còpia *incremental*.
1. Respon: quines de les còpies fetes caldran per fer una restauració?
1. Simula un *crash* de l'SGBD.
1. Restaura les còpies de seguretat necessàries.
1. Verifica que s'han recuperat les dades correctament.

### Restauració d'un moment determinat

1. Fes una còpia de seguretat *completa* de la base de dades, si cal, o recupera l'anterior.
1. Modifica alguna dada de la base de dades.
1. Respon: quin mecanisme proporciona el teu SGBD per recuperar les dades que no s'han desat en una còpia de seguretat?
1. Simula un *crash* de l'SGBD.
1. Utilitzant els mètodes de recuperació del teu SGBD, recupera la base de dades a l'estat anterior al *crash*
1. Verifica que s'han recuperat les dades correctament.
