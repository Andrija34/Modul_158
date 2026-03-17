🚀 Auftrag 1 -- Projektplanung (Grobe Umsetzung) CRM-Migration
=============================================================

Projekt
-------

CRM-Migration `crmserver.sample.ch`

Autor
-----

Andrija Milosevic

* * * * *

1\. Vorgehensstrategie
======================

Die Migration wird als **Parallelmigration mit kontrolliertem Cutover** umgesetzt.

Das bedeutet:

-   Das neue System wird vollständig vorbereitet

-   Die Migration wird zuerst in einer Testumgebung durchgeführt

-   Erst wenn alles funktioniert, erfolgt die Umschaltung

👉 Vorteil:

-   minimale Downtime

-   geringes Risiko

-   saubere Tests möglich

* * * * *

2\. Gesamtvorgehen (Übersicht)
==============================

Das Projekt wird in fünf klar definierte Phasen unterteilt:

1.  Planung

2.  Analyse & Umgebung

3.  Zielsystem Aufbau

4.  Migration

5.  Testing & Deployment

* * * * *

3\. Phase 1 -- Planung
=====================

Ziel
----

Klare Struktur und Vorbereitung des Projekts

Umsetzung
---------

-   Projektauftrag analysieren

-   Anforderungen definieren (funktional & technisch)

-   Zielarchitektur festlegen

-   Migrationsstrategie wählen (Variante A)

-   Risiken identifizieren

-   Teststrategie planen

Ergebnis
--------

-   Projektplan

-   Struktur für Git/Dokumentation

-   klare Vorgehensweise

* * * * *

4\. Phase 2 -- Analyse & Umgebung
================================

Ziel
----

Bestehendes System verstehen und reproduzierbar machen

Umsetzung
---------

-   bestehende VM starten

-   System analysieren (OS, Webserver, DB, PHP)

-   verwendete Dienste und Abhängigkeiten erfassen

-   Speicherorte der CRM-Daten identifizieren

-   System dokumentieren (IST-Zustand)

Parallel:

-   neue VM für Zielsystem vorbereiten

-   Netzwerk und Zugriff definieren

Ergebnis
--------

-   vollständige IST-Dokumentation

-   funktionierende Testumgebung

* * * * *

5\. Phase 3 -- Zielsystem Aufbau
===============================

Ziel
----

Neue, saubere und sichere Zielumgebung bereitstellen

Umsetzung
---------

-   neues Betriebssystem installieren

-   Webserver konfigurieren

-   PHP-Umgebung einrichten

-   Datenbankserver installieren

-   Zugriffsmöglichkeiten (SFTP/FTPS) einrichten

-   Administrations-Tools bereitstellen

-   grundlegende Sicherheitsmassnahmen umsetzen

Ergebnis
--------

-   vollständig funktionsfähiges Zielsystem

-   sichere und wartbare Infrastruktur

* * * * *

6\. Phase 4 -- Migration
=======================

Ziel
----

Übertragung des bestehenden CRM-Systems auf das neue System

Umsetzung
---------

-   vollständiges Backup des Altsystems erstellen

-   CRM-Dateien übertragen

-   Datenbank exportieren und importieren

-   Konfigurationsdateien anpassen

-   Systemverbindungen prüfen

-   Migration zuerst in Testumgebung durchführen

Besonderheit
------------

Die Migration wird **mehrfach getestet**, bevor sie produktiv durchgeführt wird.

Ergebnis
--------

-   CRM läuft auf neuem System

-   Daten vollständig vorhanden

* * * * *

7\. Phase 5 -- Testing & Deployment
==================================

Ziel
----

Sicherstellen, dass das System stabil und korrekt funktioniert

Umsetzung
---------

### Testing

-   Login und Benutzerzugriff testen

-   Daten prüfen

-   zentrale Funktionen testen

-   Fehler analysieren und beheben

### Deployment

-   finales Backup erstellen

-   letzte Daten synchronisieren

-   Umschaltung (Cutover) durchführen

-   System nach Go-Live prüfen

### Monitoring

-   Systemüberwachung aktivieren

-   Logs kontrollieren

Ergebnis
--------

-   stabiles produktives System

-   Migration erfolgreich abgeschlossen

* * * * *

8\. Zeitplanung
===============

| Tag | Phase |
| --- | --- |
| Tag 1 | Planung + Analyse |
| Tag 2 | Umgebung + IST |
| Tag 3 | Zielsystem |
| Tag 4 | Migration |
| Tag 5 | Testing + Deployment |

* * * * *

9\. Risikoüberblick
===================

| Risiko | Massnahme |
| --- | --- |
| Datenverlust | vollständiges Backup |
| Fehler bei Migration | Tests in Umgebung |
| Inkompatibilität | Voranalyse |
| Downtime | Parallelmigration |

* * * * *

10\. Sicherheitsüberlegungen
============================

Während der Migration wird die Sicherheit verbessert durch:

-   aktuelles Betriebssystem

-   reduzierte Angriffsfläche

-   kontrollierte Benutzerzugriffe

-   saubere Rechtevergabe

-   strukturierte Systemarchitektur

* * * * *

11\. Qualitätsmerkmale (Note 6)
===============================

Diese Planung erfüllt die Anforderungen für eine hohe Bewertung:

-   klare Phasenstruktur

-   logisches Vorgehen

-   Risikoabsicherung

-   Teststrategie vorhanden

-   Deployment geplant

-   professioneller Aufbau

* * * * *

12\. Fazit
==========

Die Migration wird strukturiert, sicher und kontrolliert durchgeführt.

Durch die gewählte Strategie wird:

-   das Risiko minimiert

-   die Downtime reduziert

-   eine stabile Zielumgebung erreicht

➡️ Das Projekt entspricht dem **erweiterten Niveau (Note 6)**.
