# Übung – Grundelemente der Migration  

---

## 1. Zwei Gründe für eine Software-Migration

Eine Software-Migration wird notwendig, wenn:

1. **Bestehende Systeme neue Hard- und Software-Anforderungen nicht mehr erfüllen**  
   → Das System ist veraltet oder nicht mehr leistungsfähig genug.

2. **Technologische Veränderungen in der IT-Umgebung stattfinden**  
   → Änderungen an Hardware oder Infrastruktur ziehen weitere Anpassungen nach sich.

---

## 2. Definition des Begriffs „Migration“

Im Skript wird Migration wie folgt definiert:

> Migration ist ein Verfahren, bei dem ein Teil eines Systems in ein anderes übertragen wird, wobei möglichst alle Daten von einem Ursprungsort an einen neuen Zielort verschoben werden, ohne dass sich die Funktionalität verändert.

Wesentliche Merkmale:
- Übertragung in eine neue Umgebung  
- Funktionalität bleibt identisch  
- Keine Neuinstallation der Daten erforderlich  

---

## 3. Bereich im Software-Engineering

Die **Software-Migration** gehört zum Bereich der:

> **Software-Erhaltung**

Innerhalb des Software-Engineering wird unterschieden zwischen:
- Software-Entwicklung  
- Software-Erhaltung  

Zur Software-Erhaltung zählen:
- Software-Wartung  
- Software-Evolution  
- Software-Sanierung  
- Software-Migration  

---

## 4. Beziehung zwischen Hard- und Software-Migration

Hard- und Software-Migration stehen in enger Beziehung:

- Bei einer **Hardware-Migration** wird ein System auf neue Hardware übertragen.
- In der Regel muss danach auch die **Software angepasst oder aktualisiert** werden.
- Deshalb gehen Hardware- und Software-Migration häufig Hand in Hand.

---

## 5. Was darf nicht mit einer Migration vermischt werden – und warum?

Migration darf **niemals mit funktionalen Veränderungen** vermischt werden.

Begründung:
- Ein migriertes System muss funktional identisch mit dem ursprünglichen System sein.
- Nur so kann ein direkter Vergleich und Test gegen das Ursprungssystem erfolgen.
- Änderungen sollten erst nach vollständig abgeschlossener Migration erfolgen.

---

## 6. Ziel des Reengineering

Reengineering zielt auf:

> Die Verbesserung der Software-Qualität

Unterschied zur Migration:
- Migration → Übertragung in neue Umgebung  
- Reengineering → Qualitätsverbesserung in derselben Umgebung  

Die Funktionalität bleibt dabei ebenfalls unverändert.

---

## 7. Definition von Reverse Engineering

Reverse Engineering bedeutet:

> Das Ableiten oder Nachdokumentieren von Informationen über ein bestehendes System.

Zweck:
- Analyse des Systems  
- Dokumentation in Form von Diagrammen, Tabellen oder Text  
- Grundlage für Weiterentwicklung oder Migration  

Das bestehende System selbst bleibt dabei unverändert.

---
