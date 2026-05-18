# **INFORME TÈCNIC: PLA DE TRANSFORMACIÓ DIGITAL**

**Client:** TransRàpid S.L.

**Elaborat per:** \[Nom de la teva empresa de serveis informàtics\]

**Data:** 18 de maig de 2026

---

## **1\. Diagnòstic de Situació: El "Caos de Dades"**

L'ús d'un únic fitxer Excel per gestionar tota la logística de TransRàpid S.L. ha arribat al seu límit operatiu. S'han identificat els següents "punts de dolor":

* **Risc de corrupció i pèrdua:** Un fitxer tan gran té un alt risc de quedar malmès, perdent anys d'històric de factures i manteniments.  
* **Manca de multiusuari:** Només una persona pot editar el fitxer alhora. Si algú l'oblida obert, bloqueja la feina de l'administrador i del cap de logística.  
* **Inconsistència de dades (Errors humans):** No hi ha validació. Es poden introduir rutes duplicades o xifres de benzina errònies sense cap control.  
* **Baixa escalabilitat:** Amb 6 vehicles, l'Excel ja és lent; si la flota creix, el sistema col·lapsarà totalment.  
* **Inexistència de còpies de seguretat:** Si el disc dur de l'ordinador on resideix l'Excel falla, l'empresa s'atura completament.  

  [https://docs.google.com/spreadsheets/d/1iK7LmBG2GEtCZjjejXMzNE\_klX5864vY4-mpZ8CGKWY/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1iK7LmBG2GEtCZjjejXMzNE_klX5864vY4-mpZ8CGKWY/edit?usp=sharing)

---

## **2\. Proposta de Maquinari (Hardware)**

Per modernitzar l'operativa, proposem una infraestructura híbrida que prioritza la mobilitat i la resistència.

### **A l'Oficina (Seu Central)**

* **Servidor:** Es recomana una solució **Cloud (Azure o AWS)** en lloc d'un servidor físic local per estalviar costos de manteniment i electricitat, i garantir disponibilitat 24/7.  
* **Equips de sobretaula (2 unitats):** Per a l'administrador i el cap de logística.  
  * *Especificacions:* Processador Intel i5, 16GB RAM, Disc SSD 512GB, Monitor de 24" (crucial per a la visualització de rutes i factures).  
  * *Preu estimat:* 750 €/unitat.

### **En Ruta (Flota de 2 camions i 4 furgonetes)**

* **Dispositius (6 unitats):** Tablets robustes (Ruggedized) de 8 polzades amb protecció contra caigudes i pols (Certificació IP67).  
* **Connectivitat:** Targetes SIM amb dades **5G** per a la sincronització en temps real de l'albarà digital i seguiment GPS.  
* *Preu estimat:* 350 €/unitat (tablet) \+ Suports de vehicle professionals (50 €/u).

---

## **3\. Estudi Comparatiu de Programari (Software)**

| Característica | Opció A: Programari Lliure (Odoo Community) | Opció B: SaaS Comercial (SAP Business One / TMS Específic) |
| :---- | :---- | :---- |
| **Llicenciament** | Gratuït (mòduls bàsics). Pagament per manteniment. | Cost per usuari mensual (SaaS). |
| **Personalització** | Molt alta. Podem crear mòduls a mida per a TransRàpid. | Limitada a les opcions del proveïdor. |
| **Suport** | A càrrec de la nostra empresa informàtica. | Directe del fabricant del software. |
| **Implementació** | Més lenta (requereix configuració inicial). | Més ràpida (configuració estàndard). |
| **Ideal per a...** | Pimes que volen control total del codi i dades. | Empreses que volen una solució "claus en mà". |

**Recomanació:** Proposem **Odoo amb mòduls de Flota i Inventari**, ja que permet integrar la facturació amb el manteniment dels camions sense dependre d'unes quotes mensuals elevades de SAP.

---

## **4\. Seguretat i Còpies de Seguretat (Backup)**

Per garantir que les dades de facturació i rutes no es perdin mai, s'implementarà la **Regla 3-2-1**:

1. **3 Còpies:** Una en producció, una en un servidor de backup i una fora de la oficina.  
2. **2 Suports diferents:** Disc dur local a l'oficina per a recuperació ràpida i Cloud Storage.  
3. **1 Còpia fora de línia:** Còpia diària en un núvol xifrat (tipus Backblaze o Google Cloud Storage) en un centre de dades geogràficament distant.

---

## **5\. Pressupost de Digitalització**

| Concepte | Descripció | Preu Unitari | Total |
| :---- | :---- | :---- | :---- |
| **Maquinari Oficina** | 2 PC de sobretaula \+ Monitors | 750,00 € | 1.500,00 € |
| **Maquinari Ruta** | 6 Tablets robustes \+ Suports | 400,00 € | 2.400,00 € |
| **Software** | Instal·lació i Parametrització Odoo | 1.200,00 € | 1.200,00 € |
| **Serveis Cloud** | Hosting Servidor \+ Backup (1r any) | 600,00 € | 600,00 € |
| **Formació** | 10 hores de formació per a treballadors | 45,00 € | 450,00 € |
| **TOTAL (base imposable)** |  |  | **6.150,00 €** |

---

## **6\. Viabilitat i Conclusions**

El projecte és tècnicament viable i necessari. La inversió inicial de 6.150 € s'amortitzarà en menys d'un any gràcies a l'eliminació d'errors en la facturació, l'estalvi de temps del cap de logística i la millora en la conservació dels vehicles mitjançant el control de manteniment automàtic.

TransRàpid S.L. deixarà de ser una empresa en risc per "caos de dades" per convertir-se en una operadora logística digitalment eficient.

