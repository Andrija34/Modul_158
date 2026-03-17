Auftrag 1 -- Projektplan
=======================

**Projekt:** CRM-Migration `crmserver.sample.ch`\
**Modul:** M158 LB2\
**Autor:** Andrija [Nachname]\
**Version:** 1.0\
**Datum:** [Datum einfügen]

* * * * *

1\. Ausgangslage
----------------

Das bestehende CRM-System `crmserver.sample.ch` liegt als **on-prem VM-Export** vor.\
Gemäss Projektauftrag soll das System:

-   auf ein **neues Betriebssystem** migriert werden

-   mit **neuem Webserver und Datenbankserver** betrieben werden

-   **vollständig migriert** werden

-   in Bezug auf **Sicherheit verbessert** werden

Zusätzlich wird erwartet, dass eine **Testumgebung** aufgebaut wird, damit das bestehende System analysiert, dokumentiert und grafisch dargestellt werden kann. Alle Arbeitsschritte müssen nachvollziehbar dokumentiert werden, inklusive **Begründungen, Grafiken, Code, Eingaben/Ausgaben sowie Fehler und deren Behebung**.

* * * * *

2\. Projektziel
---------------

Ziel des Projekts ist die erfolgreiche Migration des bestehenden CRM-Systems auf eine moderne, sicherere und wartbare Zielumgebung mit möglichst kurzer Downtime.

### Hauptziele

1.  Bestehendes CRM-System in einer **Testumgebung bereitstellen**

2.  **IST-Analyse** von System, Diensten, Datenbank und Abhängigkeiten durchführen

3.  **SOLL-Architektur** definieren

4.  Neue Zielumgebung mit folgenden Komponenten aufbauen:

    -   DNS

    -   Webserver

    -   PHP

    -   MySQL/MariaDB

    -   PhpMyAdmin oder Adminer

    -   SFTP oder FTPS

5.  CRM-Daten und Webanwendung vollständig migrieren

6.  Backup-, Monitoring- und Testkonzept umsetzen

7.  Deployment mit kurzer Unterbrechung planen und dokumentieren

### Qualitätsziele für Note 6

Um das Niveau **„erweitert / Note 6"** zu erreichen, wird das Projekt nicht nur funktional umgesetzt, sondern auch sauber geplant, begründet, getestet und abgesichert:

-   klare **Projektphasen**

-   nachvollziehbare **Entscheidungsbegründungen**

-   **Risikoanalyse** mit Massnahmen

-   **Rollback-Plan**

-   **Testkatalog**

-   **Sicherheitsmassnahmen**

-   **Monitoring**

-   saubere **Git-Dokumentation**

-   aussagekräftige **IST-/SOLL-Diagramme**

* * * * *

3\. Projektumfang
-----------------

Der Projektumfang orientiert sich an den 14 geforderten Dokumentationsabschnitten des Projektauftrags:\
Projektplan, Architekturdiagramm IST/SOLL, Umgebung, DNS, Webserver, PHP, DB-Server, PhpMyAdmin/Adminer, SFTP/FTPS, WebApp-Migration, Backup, Testing, Monitoring, Deployment.

### In Scope

-   Testumgebung bereitstellen

-   Bestandssystem analysieren

-   neue Linux-VM erstellen

-   Webstack installieren und konfigurieren

-   Datenbank migrieren

-   CRM-Dateien migrieren

-   Zugriff testen

-   Backup einrichten

-   Monitoring einrichten

-   Deployment dokumentieren

### Out of Scope

-   komplette funktionale Neuentwicklung des CRM

-   Individualentwicklung neuer CRM-Features

-   produktiver Parallelbetrieb über längere Zeit

-   Migration auf ein komplett anderes ERP im Hauptszenario

* * * * *

4\. Migrationsvarianten
-----------------------

Im Auftrag sind zwei Varianten vorgesehen:\
**A)** Migration auf die neueste Version von Vtiger\
**B)** Migration auf ein anderes Open-Source-ERP, z. B. OpenERP, inklusive Datenmigration.

### Bewertung der Varianten

#### Variante A -- Upgrade/Migration auf aktuelle Vtiger-Version

**Vorteile**

-   geringeres Migrationsrisiko

-   bestehende Prozesse eher kompatibel

-   weniger Schulungsaufwand

-   schnellere Umsetzung

-   geringere Ausfallzeit

**Nachteile**

-   Altlasten evtl. teilweise weitergeführt

-   evtl. technische Einschränkungen des Altsystems

#### Variante B -- Migration auf anderes Open-Source-ERP

**Vorteile**

-   strategisch grössere Modernisierung möglich

-   evtl. bessere Zukunftsfähigkeit

**Nachteile**

-   deutlich höherer Aufwand

-   komplexe Datenmigration

-   höheres Fehlerrisiko

-   längere Testphase

-   höhere Kosten

-   grösserer Schulungsbedarf

### Entscheidung

Für dieses Projekt wird **Variante A** empfohlen:\
**Migration auf eine aktuelle, stabile Vtiger-Zielumgebung**.

### Begründung

Da das System **während 5--6 Tagen pro Woche aktiv genutzt wird** und der **Ausfall möglichst kurz** bleiben soll, ist die risikoärmere und schneller umsetzbare Variante A klar besser geeignet.

* * * * *

5\. Projektorganisation
-----------------------

### Rollen

| Rolle | Verantwortlich |
| --- | --- |
| Projektleiter / Umsetzer | Andrija [Nachname] |
| Auftraggeber / Kunde | Lehrperson / fiktiver Kunde |
| Qualitätssicherung | Selbstkontrolle + Lehrperson |
| Dokumentation | Andrija [Nachname] |

### Arbeitsmittel

-   Git / GitLab

-   VM-Umgebung

-   Linux Server

-   SSH / SFTP

-   MariaDB / MySQL

-   Webserver

-   PHP

-   Adminer oder PhpMyAdmin

-   Monitoring-Tool

-   Markdown-Dokumentation

* * * * *

6\. Projektphasen
-----------------

Die Planung orientiert sich an den fünf im Auftrag genannten Phasen:\
**Planung, Umgebung, Zielsystem, Migration, Tests**.

### Phase 1 -- Planung

**Ziele**

-   Auftrag analysieren

-   Projektplan erstellen

-   Anforderungen festhalten

-   Risiken identifizieren

-   Testkatalog vorbereiten

-   IST-/SOLL-Konzept vorbereiten

**Ergebnisse**

-   Projektplan

-   Anforderungsliste

-   Risikoanalyse

-   Testkonzept

-   Zeitplanung

* * * * *

### Phase 2 -- Umgebung

**Ziele**

-   Export des Bestandssystems in Testumgebung bereitstellen

-   neue VM vorbereiten

-   Netzwerkparameter festlegen

-   Basis-OS installieren

-   Snapshots erstellen

**Ergebnisse**

-   lauffähige Testumgebung

-   neue Ziel-VM

-   dokumentierte Systembasis

* * * * *

### Phase 3 -- Zielsystem

**Ziele**

-   DNS konfigurieren

-   Webserver installieren

-   PHP einrichten

-   DB-Server einrichten

-   Adminer/PhpMyAdmin installieren

-   SFTP/FTPS konfigurieren

-   Grundsicherheit umsetzen

**Ergebnisse**

-   einsatzbereites Zielsystem

-   dokumentierte Konfiguration

-   abgesicherte Services

* * * * *

### Phase 4 -- Migration

**Ziele**

-   vollständiges Backup erstellen

-   CRM-Dateien übernehmen

-   Datenbank exportieren/importieren

-   Konfigurationsdateien anpassen

-   Verbindungen, Pfade und Rechte prüfen

-   Downtime-Minimierung sicherstellen

**Ergebnisse**

-   migriertes CRM-System auf Zielumgebung

-   dokumentierte Migration

-   Rollback-Möglichkeit

* * * * *

### Phase 5 -- Tests

**Ziele**

-   technische Tests

-   Funktionstests

-   Benutzerbezogene Tests

-   Sicherheitsprüfung

-   Monitoring prüfen

-   Deployment-Freigabe vorbereiten

**Ergebnisse**

-   Testprotokolle

-   Fehlerliste und Korrekturen

-   Freigabe für produktive Umschaltung

* * * * *

7\. Meilensteine
----------------

| Meilenstein | Beschreibung | Ergebnis |
| --- | --- | --- |
| M1 | Auftrag analysiert | Projektplan freigegeben |
| M2 | IST-System in Testumgebung lauffähig | IST-Analyse abgeschlossen |
| M3 | Zielsystem bereit | Web/DB/PHP/DNS/SFTP laufen |
| M4 | Migration technisch abgeschlossen | CRM auf Zielsystem verfügbar |
| M5 | Tests erfolgreich | Abnahmebereit |
| M6 | Deployment dokumentiert | Projekt abgeschlossen |

* * * * *

8\. Zeitplanung
---------------

### Vorschlag für 5 Projekttage

| Tag | Arbeitspaket |
| --- | --- |
| Tag 1 | Projektplanung, IST-Analyse, Bestandssystem starten, Dokumentationsstruktur erstellen |
| Tag 2 | Neue VM aufsetzen, OS konfigurieren, DNS/Webserver/PHP vorbereiten |
| Tag 3 | Datenbankserver, Adminer/PhpMyAdmin, SFTP/FTPS, Sicherheitsbasis konfigurieren |
| Tag 4 | Backup, Datei- und Datenmigration, Konfigurationsanpassungen, erste Funktionstests |
| Tag 5 | Testkatalog vollständig durchführen, Monitoring einrichten, Deployment- und Rollback-Doku abschliessen |

### Detaillierte Aufwandsschätzung

| Arbeitspaket | Aufwand |
| --- | --- |
| Projektplanung und Analyse | 4 h |
| IST-Dokumentation / Diagramm | 3 h |
| Zielsystem aufbauen | 6 h |
| Web-/PHP-/DB-Konfiguration | 5 h |
| Migration | 5 h |
| Backup / Monitoring | 3 h |
| Testing / Fehlerbehebung | 5 h |
| Deployment-Dokumentation | 3 h |
| **Total** | **34 h** |

* * * * *

9\. Kostenabschätzung
---------------------

Da es sich um ein Schulprojekt handelt, werden die Kosten als **Modellrechnung** dargestellt.

| Position | Aufwand | Ansatz | Kosten |
| --- | --- | --- | --- |
| Analyse und Planung | 4 h | CHF 120/h | CHF 480 |
| Aufbau Zielsystem | 11 h | CHF 120/h | CHF 1'320 |
| Migration | 5 h | CHF 120/h | CHF 600 |
| Testing / QS | 5 h | CHF 120/h | CHF 600 |
| Dokumentation / Deployment | 6 h | CHF 120/h | CHF 720 |
| **Total Dienstleistung** | **31 h** |  | **CHF 3'720** |

### Infrastrukturkosten

Im Labor / Schulumfeld vernachlässigbar bzw. bereits vorhanden.

### Empfehlung an den Kunden

Variante A ist wirtschaftlich sinnvoller, da sie mit tieferem Risiko und tieferen Kosten verbunden ist.

* * * * *

10\. Anforderungen
------------------

### Funktionale Anforderungen

-   CRM muss nach Migration erreichbar sein

-   bestehende Daten müssen vollständig vorhanden sein

-   Benutzeranmeldung muss funktionieren

-   zentrale CRM-Funktionen müssen nutzbar sein

-   Dateiübertragung für Administration muss möglich sein

### Nicht-funktionale Anforderungen

-   möglichst kurze Downtime

-   höhere Sicherheit als Altumgebung

-   nachvollziehbare Dokumentation

-   testbare und wartbare Zielumgebung

-   Backup und Rollback müssen möglich sein

* * * * *

11\. Risikoanalyse
------------------

| Risiko | Auswirkung | Eintritt | Massnahme |
| --- | --- | --- | --- |
| Datenbankimport fehlerhaft | CRM unvollständig | mittel | vorgängiges Backup, Testimport in Lab |
| PHP-Version inkompatibel | Anwendung startet nicht | mittel | Kompatibilität vorab prüfen, Version dokumentieren |
| Rechte-/Pfadfehler | Seitenfehler / Uploadfehler | hoch | Dateirechte dokumentieren und testen |
| DNS-/Hostfehler | System nicht erreichbar | mittel | lokale Hosts-Tests vor Umschaltung |
| Downtime zu lang | Benutzerbetrieb gestört | mittel | Vorab-Migration im Test, Cutover-Checkliste |
| Fehlende Rollback-Option | hohe Störung | tief | Snapshot + Backup + Restore-Test |

* * * * *

12\. Sicherheitskonzept
-----------------------

Zur Erhöhung der Sicherheit werden folgende Massnahmen umgesetzt:

-   neues, aktuelles Betriebssystem

-   unnötige Dienste deaktivieren

-   SSH/SFTP abgesichert konfigurieren

-   starke Passwörter verwenden

-   Datenbankzugriffe auf notwendige Benutzer einschränken

-   Verzeichnis- und Dateirechte korrekt setzen

-   Administrationszugänge trennen

-   Backup regelmässig erstellen

-   Monitoring für Verfügbarkeit und Dienste einrichten

Diese Punkte unterstützen direkt die im Projektauftrag geforderte **Sicherheitsverbesserung**.

* * * * *

13\. Backup- und Rollback-Plan
------------------------------

### Backup vor Migration

Vor jedem kritischen Schritt werden folgende Sicherungen erstellt:

-   VM-Snapshot

-   Backup der CRM-Dateien

-   SQL-Dump der Datenbank

-   Sicherung relevanter Konfigurationsdateien

### Rollback

Falls die Migration fehlschlägt:

1.  produktive Umschaltung stoppen

2.  Snapshot / Backup zurückspielen

3.  DNS / Zugriff wieder auf Altsystem lenken

4.  Fehler analysieren

5.  neuen Migrationsversuch erst nach Korrektur starten

* * * * *

14\. Testkonzept
----------------

Der Projektauftrag verlangt ausdrücklich **Testing** als eigene Phase.

### Testarten

#### 1\. Infrastrukturtests

-   Server erreichbar

-   DNS-Auflösung funktioniert

-   Webserver läuft

-   PHP verarbeitet Testdatei

-   DB-Server erreichbar

-   SFTP/FTPS-Zugriff funktioniert

#### 2\. Migrationstests

-   CRM-Dateien vollständig vorhanden

-   Datenbank erfolgreich importiert

-   Konfiguration korrekt angepasst

-   Login funktioniert

-   Datensätze sichtbar

#### 3\. Funktionstests

-   Benutzeranmeldung

-   Kunden-/Kontaktansicht

-   Suchfunktion

-   Datensatz erstellen / ändern

-   Upload / Download falls vorhanden

#### 4\. Sicherheitstests

-   unnötige Standardseiten entfernt

-   Admin-Zugänge geschützt

-   Schreibrechte nur wo nötig

-   Fehlermeldungen verraten keine sensiblen Details

#### 5\. Backup-/Restore-Test

-   SQL-Dump lesbar

-   Rücksicherung testbar

-   Backup-Dateien vollständig

### Abnahmekriterien

Die Migration gilt als erfolgreich, wenn:

-   das CRM ohne kritische Fehler startet

-   Login und Kernfunktionen funktionieren

-   Daten vollständig vorhanden sind

-   Zielsystem dokumentiert ist

-   Backup und Monitoring nachweislich funktionieren

* * * * *

15\. Monitoring-Konzept
-----------------------

Gemäss Projektauftrag gehört **Monitoring** ebenfalls zum Projektumfang.

Überwacht werden:

-   Server-Verfügbarkeit

-   HTTP/HTTPS-Erreichbarkeit

-   Datenbankdienst

-   Speicherplatz

-   CPU / RAM

-   optional: Prozessüberwachung für Webserver und DB

Ziel ist, Störungen früh zu erkennen und die Betriebsfähigkeit der Zielumgebung nachzuweisen.

* * * * *

16\. Deployment-Strategie
-------------------------

Da die Ausfallzeit kurz bleiben muss, wird eine **Parallelvorbereitung mit kontrolliertem Cutover** gewählt.

### Vorgehen

1.  Zielsystem vollständig in Testumgebung vorbereiten

2.  Migration mehrfach testen

3.  finales Backup des Altsystems erstellen

4.  letzte Daten übernehmen

5.  Konfiguration final anpassen

6.  DNS/Umschaltung durchführen

7.  Smoke-Test direkt nach Umschaltung

8.  Monitoring kontrollieren

### Vorteil

-   kurze Unterbrechung

-   geringeres Risiko

-   Rollback bleibt möglich

* * * * *

17\. Dokumentationsstruktur im Git
----------------------------------

M158/\
├── 01_Projektplan/\
│   └── Projektplan.md\
├── 02_Architekturdiagramm/\
│   ├── IST.png\
│   ├── SOLL.png\
│   └── Architektur.md\
├── 03_Umgebung/\
├── 04_DNS/\
├── 05_Webserver/\
├── 06_PHP/\
├── 07_Datenbank/\
├── 08_Adminer/\
├── 09_SFTP/\
├── 10_Migration/\
├── 11_Backup/\
├── 12_Testing/\
├── 13_Monitoring/\
└── 14_Deployment/

* * * * *

18\. Fazit und Empfehlung
-------------------------

Für dieses Projekt ist die **Migration auf eine aktuelle Vtiger-Zielumgebung** die beste Wahl.\
Sie erfüllt die Anforderungen des Kunden nach:

-   vollständiger Migration

-   höherer Sicherheit

-   kurzer Ausfallzeit

-   nachvollziehbarer Dokumentation

-   realistischer Umsetzung in den geforderten Projektphasen

Mit dieser Planung ist eine strukturierte Umsetzung auf **erweitertem Niveau** möglich.

* * * * *

19\. Besonderer Hinweis zur Abgabe
----------------------------------

Auf Seite 3 steht in der Abschnittsliste **„WordPress-Migration"**, obwohl das eigentliche Projekt klar als **CRM Migration** beschrieben ist. Inhaltlich solltest du deine Dokumentation natürlich auf **CRM / Vtiger** ausrichten; das wirkt sauber und aufmerksam.
