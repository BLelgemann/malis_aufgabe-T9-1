
## Der Nutzerdatenimport von der Campus Management Software *academyFIVE* in das Bibliotheksystem *KOHA* der Macromedia Library

### Inhalt

1. [Organisationsstruktur der Macromedia Library](#macromedialibrary)  
2. [Das Macromedia Library Bibliothekssystem](#Bibliothekssystem)  
    2.1 [Hosting durch das BSZ](#Hosting)    
    2.2 [Das Bibliothekssystem Koha](#Koha)      
3. [academyFIVE – Die Campus Management Software](#academyFIVE)     
    3.1 [Funktionen](#Funktionen)         
    3.2 [Datenpflege](#Datenpflege)     
4. [Nutzerdatenimport von academyFIVE nach Koha - Probleme und Verbesserungsvorschläge](#Nutzerdatenimport)   
[Quellen](#Quellen) 

### 1. Organisationsstruktur der Macromedia Library <a name="macromedialibrary" /></a>

Die Hochschule Macromedia hat mehrere Standorte in Deutschland, mit jeweils einer physischen Bibliothek. Alle Standortbibliotheken teilen einen OPAC (Macromedia Library, 2019), der über das Open-Source-Bibliothekssystem Koha bereitgestellt wird. Da sowohl das Bibliothekspersonal als auch die IT-Abteilung je Standort in der Regel nur mit einer Person besetzt wird und die zentrale IT-Abteilung hauptsächlich mit der Wartung des Firmenservers beschäftigt ist, werden IT-bezogene Bibliotheksdienste generell durch externe Anbieter betreut. So wird das Koha bzw. die dahinterliegende Datenbank durch das Bibliotheksservice-Zentrum Baden-Württemberg (BSZ) gehostet. 
  
### 2. Das Macromedia Library Bibliothekssystem <a name="Bibliothekssystem" /></a>

#### 2.1 Hosting durch das BSZ <a name="Hosting" /></a>

Die Macromedia Library ist Mitglied des Südwestdeutschen Bibliotheksverbundes (SWB). Das daran angeschlossene Bibliotheksservice-Zentrum Baden-Württemberg (BSZ) ist, wie beschrieben, für das Hosting der mit Koha verbundenen Datenbank zuständig: 

> Das BSZ unterstützt die Bibliothek bei der Datenmigration aus vorhandenen 
> Systemen und übernimmt die Daten aus dem SWB-Verbund direkt nach
> KohaAusgerichtet an den jeweiligen Geschäftsgängen erarbeitet das BSZ 
> gemeinsam mit der Einrichtung die Konfiguration des Systems . . . Über den
> automatisierten täglichen Datenimport und Z39.50-Download werden Daten nach
> Koha übernommen. (BSZ, o.D.) 

Für die Übermittlung von Katalog-Daten wird den Mitgliedern des SWB-Verbundsystems der Katalogisierungsclient WinIBW von OCLC zur Verfügung gestellt (BSZ, o.D.).   
   
#### 2.2 Das Bibliothekssystem Koha <a name="Koha" /></a>

Koha ist ein Open-Source-Bibliothekssystem, das `gemäß den Bedingungen der GNU General Public Licence` (`Über Koha`, o.J.) weiterverbreitet und verändert werden darf. Es gibt dementsprechend eine Reihe von öffentlichen [Git Repositorien](http://git.koha-community.org/gitweb/), an denen kollaborativ gearbeitet wird (`Public Git Repositories - Koha Wiki`, 2019). Das System erfüllt (fast) alle Anforderungen, die an ein Next-Generation-Bibliotheksmanagementsystem gestellt werden, u.a. können Benutzerausweise gedruckt und der gesamte Bestell- sowie Fernleihe-Prozess abgewickelt werden. Mithilfe von Reports können zudem Datenanalysen durchgeführt und z.B. Katalog- oder Benutzerstatistiken erstellt werden (Abb 1).  

       # ----- Bild einfügen -> koha_reports.jpg 
        Abb 1: Reports in Koha (`Reports`, o.J.)

An der Macromedia Library wird Koha vor allem für die Ausleihe und die Rückgabe von Medien verwendet, für das Mahnwesen, für Inventuren und für die Bereitstellung des lokalen OPAC, inklusive Nutzerkonto. Koha ist mit dem kommerziellen Campus-Management-System *academyFIVE* (Firma Simovative) verknüpft, wodurch Studierende und Lehrende sowie Mitarbeiter_innen der Verwaltung im Bibliothekssystem automatisch per Datenmigration als Biblitheksnutzer_innen anlegt werden. Eine manuelle Nutzer_innen-Anlegung ist theoretisch möglich, allerdings muss die Person zunächst in academyFIVE eingepflegt worden sein. Im Anschluss an die Datenmigration bzw. an das manuelle Anlegen einer Person wird die jeweilige academyFIVE-ID als Personen-ID übernommen und händisch in Koha übertragen.

### 3. academyFIVE – Die Campus Management Software <a name="academyFIVE" /></a>

Laut der Simovative GmbH ist acadamyFIVE `eine Lösung auf Maß`, die `unter Berücksichtigung aller individuellen Bedürfnisse die komplexen Prozesse von Hochschulverwaltungen in einem einzigen System` (Simovative GmbH, 2020) vereint.
Das System wird dabei immer wieder an veränderte Kundenwünsche angepasst, zudem gibt es die Möglichkeit durch selbstständig durchgeführte Konfigurationen eigene Anpassungen vorzunehmen (Simovative GmbH, 2020).

#### 3.1 Funktionen  <a name="Funktionen"></a>
   
Das Hauptmenü des Camus-Management-Systems ist bei der Hochschhule Macromedia folgendermaßen aufgeteilt:
- Personen
- Kommunikation
- Angebotsgruppen & Durchführungsgruppen
- Prüfungsmanagement
- Kursmanagement
- Abgabemanagement
- Statistik und Berichte
- Dokumente
- Internetauftritt
- News
- Aufgaben
- Einstellungen (academyFive, 2020). 
        
Allerdings werden nicht alle Bereiche des Systems genutzt, wie z.B. der Bereich `Aufgaben` oder der Bereich `Kursmanagement`, da die Stunden- und Raumplanung über die Stundenplansoftware *WebUntis* organisiert wird.

Im Bereich `Kommunikation` findet die E-Mail-Kommunikation mit den Studierenden statt. Im Bereich `Personen` werden Interessenten, Bewerber, Studenten, Alumni und `Benutzerguppen` verwaltet, letzterer Menüpunkt teilt sich auf in `Aktive Autoren`, `Dozenten`, `Externe Kontakte`, `Firmen Kontakte` und `Inaktive`  (academyFive, 2020). Jede Person hat, wie bereits erwähnt, eine individuelle academyFIVE-ID. 

Hinter „Internetauftritt“ verbirgt sich die *Community* bzw. das Dozierenden- und Studierendenportal *mymacromedia.de* (Hochschule Macromedia, o. J.), welches in academyFIVE eingebettet ist. Von da aus können Studierende auf alle studienrelevanten Informationen zugreifen, sich für Prüfungen anmelden und digitale Prüfungsabgaben vornehmen. Dementsprechend ist speziell der Bereich Prüfungs- und Abgabemanagement mit der Community verbunden. Auch die News, die in der Community veröffentlicht werden, werden über academyFIVE abgesetzt.

Im Bereich `Statistik und Berichte` gibt es die Möglichkeit, Reports durchzuführen und den gesamten Datenbestand zu analysieren:

> . . . mit dem academyFIVE Reporting können Sie alle im System erfassten Daten 
> auswerten und ausgeben (CVS, XML oder MS-Excel) oder in tabellarischer Form 
> direkt im System darstellen. Mit den ausgewerteten Daten können anschließend 
> direkt Folgeprozesse (z.B. direkter Versand von E-Mails) angestoßen werden.
> Die Auswertungen finden in Echtzeit statt, wodurch die Informationen immer auf 
> dem aktuellsten Stand sind. Die Daten eines Berichts werden verschlüsselt
> bereitgestellt, so dass  sie einfach in andere Systeme der Hochschul-IT
> Landschaft (bspw. die hochschuleigene Webiste) integriert werden können.
> (Simovative GmbH, 2020)

Das System ermöglicht es somit auch, Entscheidungsprozesse zu optimieren: `Hierzu bietet Ihnen academyFIVE Analytics ein Dashboard System, mit dem beliebig viele Dashboards angelegt werden können. So werden dem einzelnen Anwender, direkt nach dem Login, alle für ihn relevanten Informationen ansprechend darstellt` (Simovative GmbH, 2020).
   
#### 3.2 Datenpflege <a name="Datenpflege" /></a>

Die Datenpflege und Aktualisierung wird durch die Verwaltungsmitarbeiter der Hochschule vorgenommen. Diese haben, je nach Zuständigkeit bzw. Abteilung, unterschiedliche Zugriffsrechte. Ferner können Studierende und Dozierende ihre Kontaktdaten über die Community selbstständig aktualisieren. Die in academyFIVE eingepflegte Hochschul-E-Mail-Adresse kann dabei nicht verändert werden.

Für den Nutzerdatenimport nach Koha werden die Daten der Mitarbeiter_innen, aktiven Teilnehmer_innen und aktiven Dozierenden regelmäßig in Koha importiert bzw. mit Koha synchronisiert.

### 4. Nutzerdatenimport von academyFIVE nach Koha - Probleme und Verbesserungsvorschläge <a name="Nutzerdatenimport" /></a>

Die E-Mail-Adressen der Nutzer_innen werden oft falsch übertragen, d.h. es werden in einigen Fällen nur die privaten E-Mail-Adressen der Teilnehmer_innen und Dozierenden übernommen oder fälschlicherweise E-Mail-Adressen von anderen Studierenden. Wie dies genau zustande kommt, ist aktuell nicht nachvollziehbar. Es wäre von großem Vorteil, wenn man durch eine (vorgeschaltete) Datenanalyse bzw. ein entsprechendes Skript herausfiltern könnte, bei welchen Nutzer_innen die Hochschuladressen fehlen. Da alle Hochschul-E-Mail-Adressen nach dem gleichen Muster aufgebaut sind - mmustermann(at)stud.macromedia.de -, könnte man zudem die Nachnamen der Nutzer_innen mit den Hochschul-E-Mail-Adressen abgleichen, um falsch zugeordnete Adressen herauszufiltern. Eine Analyse der fehlerhaften Datensätze ist ggfs. über das Erstellen von Reports möglich. Aktuell fehlt bei dem Report zur Erstellung von Benutzerstatistiken  eine Filtermöglichkeit nach E-Mail-Adressen (Abb 2). Diese Filtermöglichkeit könnte man z.B. ergänzen. Allerdings werden die Fehler dadurch nicht automatisch behoben.

        # ------Bild einfügen -> koha_benutzerstatistiken.jpg
        Abb 2: Report zu Benutzerstatistiken (`Benutzerstatistiken`, o.J.) 

Eine weitere Schwachstelle ist, dass die jeweilige academyFIVE-ID bisher händisch als Personen-ID in Koha übertragen wird (siehe Kapitel 2). Da dieses Vorgehen sehr umständlich ist, wäre es von Vorteil, wenn dieser Prozess automatisiert würde. 

### Quellen <a name="Quellen" /></a>

academyFive. (2020). Abgerufen 9. Mai 2020, von [https://ac5-prod.macromedia.de/home](https://ac5-prod.macromedia.de/home)

Benutzerstatistiken. (o. J.). Abgerufen 10. Mai 2020, von https://macromedia.bsz-bw.de:8080/cgi-bin/koha/reports/borrowers_stats.pl

BSZ. (o.D.). Koha. Abgerufen 05. Mai, 2020, von [https://www.bsz-bw.de/bibliothekssysteme/koha.html](https://www.bszbw.de/bibliothekssysteme/koha.html) 

Hochschule Macromedia. (o. J.). My Macromedia. Abgerufen 9. Mai 2020, von [https://my.macromedia.de](https://my.macromedia.de) 

Library Macromedia. (2019). Allgemeines | Bibliothek Hochschule Macromedia. Abgerufen 10. Mai 2020, von https://library.macromedia.de/bibliothek-willkommen/allgemeines/

Public Git Repositories - Koha Wiki. (2019, Oktober 1). Abgerufen 10. Mai 2020, von [https://wiki.koha-community.org/wiki/Public_Git_Repositories](https://wiki.koha-community.org/wiki/Public_Git_Repositories)

Reports. (o. J.). Abgerufen 10. Mai 2020, von https://macromedia.bsz-bw.de:8080/cgi-bin/koha/reports/reports-home.pl

Über Koha. (o. J.). Abgerufen 10. Mai 2020, von https://macromedia.bsz-bw.de:8080/cgi-bin/koha/about.pl

Simovative GmbH. (2020, April 28). Simovative GmbH | academyFIVE - Campus Management Software. Abgerufen 5. Mai 2020, von [https://www.simovative.com/de/](https://www.simovative.com/de/) 




  
