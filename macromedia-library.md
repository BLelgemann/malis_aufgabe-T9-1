
## Der Nutzerdatenimport von der Campus Management Software *academyFIVE* in das Bibliotheksystem *KOHA* der Macromedia Library

**1.** [Organisationsstruktur der Macromedia Library](#macromedialibrary) 
**2.** [Das Macromedia Library Bibliothekssystem](#Bibliothekssystem)    
       3.1 [Hosting durch das BSZ](#Hosting)    
       3.2 [Das Bibliothekssystem Koha](#Koha)      
**3.** [academyFIVE – Die Campus Management Software](#academyFIVE)     
       3.1 [Funktionen](#Funktionen)         
       3.2 [Datenpflege und Aktualisierung](#Datenpflege)     
**4.** [Nutzerdatenimport von academyFIVE nach Koha - Probleme und Verbesserungsvorschläge](#Nutzerdatenimport)      
[Quellen](#Quellen) 


### 1. Organisationsstruktur der Macromedia Library <a name="macromedialibrary" /></a>

Die Hochschule Macromedia hat insgesamt sieben Standorte in ganz Deutschland, mit jeweils einer physischen Bibliothek. Die Standortbibliotheken teilen einen OPAC, der über das Bibliothekssystem Koha bereitgestellt wird. Da sowohl das Bibliothekspersonal als auch die IT-Abteilung je Standort in der Regel nur mit einer Person besetzt wird und die zentrale IT-Abteilung hauptsächlich mit der Wartung des Firmenservers beschäftigt ist, werden IT-bezogene Bibliotheksdienste generell durch externe Anbieter gewartet. So wird das Bibliothekssystem Koha bzw. die dahinterliegende Datenbank durch das Bibliotheksservice-Zentrum Baden-Württemberg (BSZ) gehostet. 
  
### 2. Das Macromedia Library Bibliothekssystem <a name="Bibliothekssystem" /></a>

   #### 2.1 Hosting durch das BSZ <a name="Hosting" /></a>

Die Macromedia Library ist Mitglied des Südwestdeutschen Bibliotheksverbundes (SWB). Das daran angeschlossene Bibliotheksservice-Zentrum Baden-Württemberg (BSZ) ist, wie beschrieben, für das Hosting der mit Koha verbundenen Datenbank zuständig: "Das BSZ unterstützt die Bibliothek bei der Datenmigration aus vorhandenen Systemen und übernimmt die Daten aus dem SWB-Verbund direkt nach Koha" (BSZ, o.D.). Für die Übermittlung von Katalog-Daten wird den Mitgliedern des SWB-Verbundsystems der Katalogisierungsclient WinIBW von OCLC zur Verfügung gestellt (BSZ, o.D.).   
   
   #### 2.2 Das Bibliothekssystem Koha <a name="Koha" /></a>

Koha erfüllt (fast) alle Anforderungen, die an ein Next-Generation-Bibliotheksmanagementsystem gestellt werden, u.a. können Benutzerausweise gedruckt und der gesamte Bestell- sowie Fernleihe-Prozess abgewickelt werden. An der Macromedia Library wird Koha vor allem für die Ausleihe und die Rückgabe von Medien verwendet, für das Mahnwesen, für Inventuren und für die Bereitstellung des lokalen OPAC, inklusive Nutzerkonto. Koha ist mit dem Campus-Management-System *academyFive* verknüpft, wodurch Studierende und Lehrende sowie Mitarbeiter_innen der Verwaltung im Bibliothekssystem automatisch als Nutzer_innen anlegt werden. Eine manuelle Benutzer_innen-Anlegung ist theoretisch möglich, allerdings muss die Person zunächst in AC5 eingepflegt worden sein, da sich die Bibliotheksausweisnummer aus der academyFIVE-Registrierungsnummer ergibt. Diese Nummer korrespondiert mit dem Studierendenausweis oder dem Dozierendenausweis. 

### 3. academyFIVE – Die Campus Management Software <a name="academyFIVE" /></a>

   #### 3.1 Funktionen  <a name="Funktionen"></a>
   
   Das Hauptmenü des Camus-Management-Systems ist folgendermaßen aufgeteilt:
-	Personen
-	Kommunikation
-	Angebotsgruppen & Durchführungsgruppen
-	Prüfungsmanagement
-	Kursmanagement
-	Abgabemanagement
-	Statistik und Berichte
-	Dokumente
-	Internetauftritt
-	News
-	Aufgaben
-	Einstellungen (academyFive, o. J.). 

Im Bereich „Personen“ werden Interessenten, Bewerber, Studenten, Alumni und „Benutzerguppen“ verwaltet, letzterer Menüpunkt teilt sich auf in „Aktive Autoren“, „Dozenten“, „Externe Kontakte“, „Firmen Kontakte“ und „Inaktive“. Jede Person hat, wie bereits erwähnt, eine eigene Registrierungsnummer bzw. academyFIVE-Nummer. Im Bereich „Kommunikation“ findet die E-Mail-Kommunikation mit den Studierenden statt.

Hinter „Internetauftritt“ verbirgt sich die *Community* bzw. das Dozierenden- und Studierendenportal *mymacromedia.de* (Hochschule Macromedia, o. J.), welches in academyFIVE eingebettet ist. Von da aus können Studierende auf alle studienrelevanten Informationen zugreifen, sich für Prüfungen anmelden und digitale Prüfungsabgaben vornehmen. Dementsprechend ist speziell der Bereich Prüfungs- und Abgabemanagement mit der Community verbunden. Auch die News, die in der Community veröffentlicht werden, werden über academyFIVE abgesetzt.

Allerdings werden nicht alle Bereiche des Systems genutzt, wie z.B. der Bereich „Kursmanagement“, da die Stunden- und Raumplanung über die Stundenplansoftware *WebUntis* organisiert wird.
   
   #### 3.2 Datenpflege und Aktualisierung <a name="Datenpflege" /></a>

Die Datenpflege und Aktualisierung in AC5 wird durch die Verwaltungsmitarbeiter der Hochschule vorgenommen. Diese haben, je nach Zuständigkeit bzw. Abteilung, unterschiedliche Zugriffsrechte. Ferner können Studierende und Dozierende ihre Kontaktdaten über die Community selbstständig aktualisieren. Die in academyFIVE eingepflegte Hochschul-E-Mail-Adresse kann dabei nicht verändert werden.

Für den Nutzerdatenimport nach Koha werden die Daten der Mitarbeiter_innen, aktiven Teilnehmer_innen und aktiven Dozierenden regelmäßig in Koha importiert bzw. mit Koha synchronisiert.

### 4. Nutzerdatenimport von academyFIVE nach Koha - Probleme und Verbesserungsvorschläge <a name="Nutzerdatenimport" /></a>

Die E-Mail-Adressen der Nutzer_innen werden oft falsch übernommen, d.h. es werden in einigen Fällen nur die privaten E-Mail-Adressen der Teilnehmer_innen und Dozierenden übernommen oder fälschlicherweise E-Mail-Adressen von anderen Studierenden. Wie dies genau zustande kommt, ist aktuell nicht nachvollziehbar. Es wäre von großem Vorteil, wenn man durch eine (vorgeschaltete) Datenanalyse bzw. ein entsprechendes Skript herausfiltern könnte, bei welchen Nutzer_innen die Hochschuladressen fehlen. Da alle Hochschul-E-Mail-Adressen nach dem gleichen Muster aufgebaut sind (mmustermann@stud.macromedia.de), könnte man zudem die Nachnamen der Nutzer_innen mit den Hochschul-E-Mail-Adressen abgleichen, um falsch zugeordnete Adressen herauszufiltern. 

Eine weitere Schwachstelle ist, dass die Registrierungsnummer aus academyFIVE bzw. die Bibliotheksausweisnummer händisch in Koha eingetragen werden muss. Da dieses Vorgehen sehr umständlich ist, wäre es von Vorteil, wenn dieser Prozess automatisiert wird. 

### Quellen <a name="Quellen" /></a>

academyFive. (o. J.). Abgerufen 9. Mai 2020, von [https://ac5-prod.macromedia.de/home](https://ac5-prod.macromedia.de/home)

BSZ. (o.D.). Koha. Abgerufen 05. Mai, 2020, von [https://www.bsz-bw.de/bibliothekssysteme/koha.html](https://www.bszbw.de/bibliothekssysteme/koha.html) 

Simovative GmbH. (2020, April 28). Simovative GmbH | academyFIVE - Campus Management Software. Abgerufen 5. Mai 2020, von [https://www.simovative.com/de/](https://www.simovative.com/de/) 

Simovative GmbH. (2020, April 28). Simovative GmbH | academyFIVE - Campus Management Software. Abgerufen 5. Mai 2020, von [https://www.simovative.com/de/](https://www.simovative.com/de/)



  
