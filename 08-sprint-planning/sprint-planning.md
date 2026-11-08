# Sprintplanung – CRM-Modernisierung

## 1. Ziel

Diese Sprintplanung zeigt beispielhaft, wie ausgewählte User Stories aus dem priorisierten Product Backlog auf zwei Sprints verteilt werden können.

Die Planung berücksichtigt fachliche Prioritäten, Abhängigkeiten zwischen Anforderungen und übergreifende Qualitätsanforderungen.

Da es sich um eine fiktive Fallstudie handelt, werden weder eine tatsächliche Teamkapazität noch reale Aufwandswerte zugrunde gelegt.

## 2. Rahmenbedingungen

| Merkmal | Festlegung |
|---|---|
| Vorgehensmodell | Scrum-orientierte Planung |
| Sprintdauer | 2 Wochen |
| Anzahl Sprints | 2 |
| Product Backlog | 9 User Stories |
| Priorisierung | MoSCoW |
| Planungsgrundlage | Fachlicher Nutzen, Abhängigkeiten und Qualitätsanforderungen |

## 3. Sprint 1 – Grundlagen der Kundenverwaltung

**Sprintziel:**

Die grundlegenden Funktionen zur Anlage, Pflege und Suche von Kundendaten sollen fachlich ausgearbeitet werden. Dabei werden grundlegende Berechtigungsprüfungen von Beginn an berücksichtigt.

### Geplante User Stories

| ID | User Story | MoSCoW-Kategorie | Begründung |
|---|---|---|---|
| US-01 | Kundendatensatz anlegen | Must have | Grundfunktion der Kundenverwaltung |
| US-03 | Kundendaten bearbeiten | Must have | Ermöglicht die Aktualisierung bestehender Kundendaten |
| US-04 | Kundeninformationen suchen | Must have | Ermöglicht den Zugriff auf gespeicherte Kundendaten |
| US-02 | Mögliche Dubletten erkennen | Should have | Ergänzt die Neuanlage um eine Prüfung der Datenqualität |

### Übergreifende Anforderungen

Bei der fachlichen Ausarbeitung der Funktionen werden insbesondere folgende Anforderungen berücksichtigt:

- NFR-03: Zugriffssicherheit
- NFR-05: Datenintegrität
- NFR-02: Benutzbarkeit

Die grundlegenden Berechtigungsprüfungen müssen bereits bei der Anlage, Bearbeitung und Suche von Kundendaten berücksichtigt werden.

### Erwartetes Sprint-Ergebnis

Ein fachlich spezifiziertes Grundkonzept für die Kundenverwaltung mit Neuanlage, Bearbeitung, Suche und Dublettenprüfung unter Berücksichtigung grundlegender Zugriffskontrollen.

## 4. Sprint 2 – Vertriebschancen und Transparenz

**Sprintziel:**

Die Verwaltung von Vertriebschancen, die Nachvollziehbarkeit von Kundenaktivitäten und die administrative Verwaltung der CRM-Berechtigungen sollen fachlich ausgearbeitet werden.

### Geplante User Stories

| ID | User Story | MoSCoW-Kategorie | Begründung |
|---|---|---|---|
| US-06 | Vertriebschance verwalten | Must have | Grundlage für die zentrale Verwaltung von Verkaufschancen |
| US-07 | Status einer Vertriebschance aktualisieren | Must have | Baut auf der Verwaltung von Vertriebschancen auf |
| US-05 | Kundenkontakt dokumentieren | Should have | Unterstützt die Nachvollziehbarkeit von Kundenaktivitäten |
| US-08 | Vertriebschancenübersicht einsehen | Should have | Schafft Transparenz für die Vertriebsleitung |
| US-09 | Benutzerberechtigungen verwalten | Must have | Ergänzt die grundlegenden Zugriffskontrollen um die administrative Rollen- und Berechtigungsverwaltung |

### Übergreifende Anforderungen

Bei der fachlichen Ausarbeitung werden insbesondere folgende Qualitätsmerkmale berücksichtigt:

- NFR-01: Antwortzeit
- NFR-03: Zugriffssicherheit
- NFR-04: Verfügbarkeit
- NFR-05: Datenintegrität
- NFR-06: Wartbarkeit

### Erwartetes Sprint-Ergebnis

Ein fachlich ausgearbeitetes Konzept für die Verwaltung und Statuspflege von Vertriebschancen, die Dokumentation von Kundenkontakten, eine Vertriebsübersicht und die administrative Verwaltung von Benutzerberechtigungen.

## 5. Berücksichtigte Abhängigkeiten

- US-01 bildet die Grundlage für die Anlage neuer Kundendatensätze.
- US-02 ergänzt die Neuanlage aus US-01 um eine Dublettenprüfung.
- US-03 und US-04 setzen die Möglichkeit voraus, Kundendatensätze zu speichern und abzurufen.
- US-05 setzt vorhandene Kundendatensätze voraus, denen Kundenaktivitäten zugeordnet werden können.
- US-07 baut auf der Verwaltung von Vertriebschancen aus US-06 auf.
- US-08 setzt voraus, dass Vertriebschancen und deren Status im CRM gepflegt werden.
- US-09 ergänzt die bereits in Sprint 1 berücksichtigten Zugriffskontrollen um die administrative Verwaltung von Rollen und Berechtigungen.

## 6. Annahmen und Einschränkungen

Die Sprintplanung ist ein beispielhaftes Planungsartefakt und keine tatsächlich durchgeführte Scrum-Planung.

Es liegen keine Informationen zu Teamgröße, Entwicklungskapazität, Story Points oder technischen Umsetzungsvoraussetzungen vor.

Die Zuordnung der User Stories dient der Demonstration einer möglichen fachlichen Reihenfolge. Die tatsächliche Planung müsste auf Basis der verfügbaren Teamkapazität, technischer Abhängigkeiten und einer Abstimmung mit dem Product Owner erfolgen.

## 7. Fazit

Die zwei Sprints zeigen eine mögliche schrittweise Strukturierung der CRM-Modernisierung.

Sprint 1 konzentriert sich auf die Grundlagen der Kundenverwaltung und berücksichtigt bereits grundlegende Zugriffskontrollen.

Sprint 2 erweitert diese um Funktionen zur Vertriebssteuerung, Transparenz und administrativen Berechtigungsverwaltung.

Damit werden fachliche Abhängigkeiten und übergreifende Qualitätsanforderungen bereits bei der Planung berücksichtigt.