# Modul 158

Auftrag 1 -- Projektplanung CRM-Migration 
====================================================

Projekt
-------

CRM-Migration `crmserver.sample.ch`

Modul
-----

M158 -- LB2

Autor
-----

Andrija Milosevic

Version
-------

1.0

Datum
-----

17.03.2026

* * * * *

1\. Ausgangslage
================

Das bestehende CRM-System liegt als exportierte virtuelle Maschine vor und wird aktuell produktiv genutzt (Mo--Sa).

Das System soll:

-   auf ein **neues Betriebssystem** migriert werden

-   mit **neuem Webserver und Datenbankserver** betrieben werden

-   **vollständig übernommen** werden

-   in Bezug auf **Sicherheit verbessert** werden

👉 Wichtige Rahmenbedingung:\
Die **Downtime muss möglichst kurz** gehalten werden.

* * * * *

2\. Zieldefinition
==================

Hauptziel
---------

Migration des bestehenden CRM-Systems auf eine moderne, sichere und wartbare Zielumgebung mit minimaler Unterbrechung.

Teilziele
---------

-   IST-System analysieren und dokumentieren

-   SOLL-Architektur definieren

-   Zielsystem aufbauen

-   vollständige Migration durchführen

-   Testing durchführen

-   Deployment vorbereiten

* * * * *

3\. Qualitätsziele
============================================

Um eine **Note 6 (erweitert)** zu erreichen, wird das Projekt nicht nur umgesetzt, sondern professionell geplant:

-   klare Struktur in **5 Phasen**

-   nachvollziehbare **Begründungen**

-   **Risikoanalyse + Massnahmen**

-   **Rollback-Plan**

-   detailliertes **Testkonzept**

-   **Sicherheitskonzept**

-   **Monitoring**

-   saubere **Git-Dokumentation**

* * * * *

4\. Projektstrategie
====================

Gewählte Strategie: Parallelmigration mit Cutover
-------------------------------------------------

Das neue System wird vollständig vorbereitet, getestet und erst am Schluss aktiviert.

Vorteile
--------

-   minimale Downtime

-   geringes Risiko

-   saubere Tests möglich

* * * * *

5\. Migrationsvarianten
=======================

Variante A -- Vtiger Upgrade (gewählt)
-------------------------------------

**Vorteile**

-   schneller umsetzbar

-   weniger Risiko

-   weniger Schulung notwendig

-   kurze Downtime

**Nachteile**

-   evtl. Altlasten

* * * * *

Variante B -- neues ERP
----------------------

**Nachteile**

-   hoher Aufwand

-   komplexe Migration

-   hohes Risiko

-   lange Testphase

* * * * *

Entscheidung
------------

➡️ Variante A wird gewählt, da sie die Anforderungen (Zeit, Risiko, Stabilität) optimal erfüllt.

* * * * *

6\. Projektphasen
=================

Phase 1 -- Planung
-----------------

-   Auftrag analysieren

-   Anforderungen definieren

-   Risiken identifizieren

-   Testkonzept erstellen

👉 Ergebnis: Projektplan

* * * * *

Phase 2 -- Umgebung
------------------

-   bestehendes System starten (VM)

-   neue VM erstellen

-   Netzwerk konfigurieren

👉 Ergebnis: Test- und Zielumgebung bereit

* * * * *

Phase 3 -- Zielsystem
--------------------

-   DNS konfigurieren

-   Webserver installieren

-   PHP einrichten

-   Datenbankserver einrichten

-   SFTP konfigurieren

👉 Ergebnis: betriebsbereites Zielsystem

* * * * *

Phase 4 -- Migration
-------------------

-   Backup erstellen

-   Datenbank exportieren/importieren

-   Dateien übertragen

-   Konfiguration anpassen

👉 Ergebnis: CRM läuft auf neuem System

* * * * *

Phase 5 -- Testing
-----------------

-   Funktionstests

-   Sicherheitstests

-   Monitoring prüfen

👉 Ergebnis: Abnahmebereit

* * * * *

7\. Zeitplanung
===============

| Tag | Aufgabe |
| --- | --- |
| 1 | Planung + IST-Analyse |
| 2 | Umgebung + VM |
| 3 | Zielsystem |
| 4 | Migration |
| 5 | Testing + Deployment |

* * * * *

8\. Aufwandsschätzung
=====================

| Aufgabe | Stunden |
| --- | --- |
| Planung | 4 h |
| Umgebung | 5 h |
| Zielsystem | 6 h |
| Migration | 5 h |
| Testing | 5 h |
| Dokumentation | 4 h |
| **Total** | **29 h** |

* * * * *

9\. Kosten (Modell)
===================

| Bereich | Kosten |
| --- | --- |
| Planung | 480 CHF |
| Umsetzung | 1320 CHF |
| Migration | 600 CHF |
| Testing | 600 CHF |
| Dokumentation | 720 CHF |
| **Total** | **3720 CHF** |

* * * * *

10\. Anforderungen
==================

Funktional
----------

-   CRM startet fehlerfrei

-   Login funktioniert

-   Daten vollständig vorhanden

Nicht-funktional
----------------

-   kurze Downtime

-   sichere Umgebung

-   dokumentiert

* * * * *

11\. Risikoanalyse
==================

| Risiko | Auswirkung | Lösung |
| --- | --- | --- |
| Datenverlust | kritisch | Backup |
| DB Fehler | hoch | Testmigration |
| PHP inkompatibel | mittel | Version prüfen |
| Downtime zu lang | hoch | Vorbereitung |

* * * * *

12\. Sicherheitskonzept
=======================

-   aktuelles Betriebssystem

-   unnötige Dienste deaktivieren

-   sichere Passwörter

-   eingeschränkte DB-Zugriffe

-   korrekte Dateirechte

-   getrennte Admin-Zugänge

* * * * *

13\. Backup & Rollback
======================

Backup
------

-   VM Snapshot

-   Datenbank Export

-   Dateisicherung

Rollback
--------

-   Snapshot zurückspielen

-   DNS zurücksetzen

-   Fehler analysieren

* * * * *

14\. Testkonzept
================

Tests
-----

-   Login funktioniert

-   Daten vorhanden

-   CRM Funktionen laufen

-   Upload/Download

Abnahmekriterien
----------------

-   keine kritischen Fehler

-   Daten vollständig

-   System stabil

* * * * *

15\. Monitoring
===============

Überwachung von:

-   Server

-   Webserver

-   Datenbank

-   CPU / RAM

Ziel: frühzeitige Fehlererkennung

* * * * *

16\. Deployment
===============

Vorgehen
--------

1.  System vorbereiten

2.  Migration testen

3.  finales Backup

4.  Umschaltung (Cutover)

5.  Tests durchführen

* * * * *

17\. Git-Struktur
=================

M158/\
├── 01_Projektplan/\
├── 02_Architektur/\
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

18\. Fazit
==========

Die gewählte Lösung erfüllt alle Anforderungen:

-   geringe Downtime

-   hohe Sicherheit

-   saubere Migration

-   nachvollziehbare Dokumentation

➡️ Damit wird das Projekt auf **erweitertem Niveau (Note 6)** umgesetzt.

dieses ReadME wurde mit hilfe von ChatGPT erstellt
