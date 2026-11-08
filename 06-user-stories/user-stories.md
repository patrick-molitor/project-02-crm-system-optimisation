# User Stories – CRM-Modernisierung

## 1. Ziel

Dieses Dokument beschreibt ausgewählte User Stories für die geplante CRM-Modernisierung.

Die User Stories konkretisieren ausgewählte funktionale Anforderungen aus Sicht der Benutzer. Die Akzeptanzkriterien beschreiben überprüfbare Bedingungen für die jeweilige Umsetzung.

Da es sich um eine fiktive Fallstudie handelt, sind die Stories und Kriterien fachliche Vorschläge, die in einem realen Projekt mit den Stakeholdern abgestimmt werden müssten.

## 2. User Stories

### US-01: Kundendatensatz anlegen

**User Story**

Als Vertriebsmitarbeiter möchte ich einen neuen Kundendatensatz anlegen können, damit ich neue Kunden zentral im CRM erfassen kann.

**Zugehörige Anforderungen:** BR-01, BR-03, FR-01  
**Zugehöriger Use Case:** UC-01  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-01.1:** Gegeben sei ein angemeldeter und berechtigter Benutzer, wenn er die erforderlichen Kundendaten eingibt und speichert, dann wird ein neuer Kundendatensatz angelegt.
- **AC-01.2:** Wenn mindestens ein Pflichtfeld fehlt, dann weist das System auf die fehlenden Angaben hin und speichert den Datensatz nicht.
- **AC-01.3:** Wenn die Speicherung erfolgreich ist, dann zeigt das System eine Bestätigung an und stellt den angelegten Datensatz dar.

### US-02: Mögliche Dubletten erkennen

**User Story**

Als Vertriebsmitarbeiter möchte ich vor dem Anlegen eines Kunden auf mögliche Dubletten hingewiesen werden, damit ich doppelte Kundendatensätze vermeiden kann.

**Zugehörige Anforderungen:** BR-01, FR-03  
**Zugehöriger Use Case:** UC-01  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-02.1:** Wenn die eingegebenen Kundendaten anhand der festgelegten Identifikationsmerkmale einem bestehenden Datensatz ähneln, dann zeigt das System einen Hinweis auf eine mögliche Dublette an.
- **AC-02.2:** Der Hinweis enthält die fachlich freigegebenen Vergleichsinformationen zum möglichen bestehenden Datensatz.
- **AC-02.3:** Der Benutzer kann den bestehenden Datensatz prüfen, bevor er über das weitere Vorgehen entscheidet.

**Offener Punkt:** Die Identifikationsmerkmale und Regeln für die Fortsetzung einer Neuanlage müssen fachlich festgelegt werden.

### US-03: Kundendaten bearbeiten

**User Story**

Als Vertriebsmitarbeiter möchte ich bestehende Kundendaten aktualisieren können, damit die Kundeninformationen aktuell bleiben.

**Zugehörige Anforderungen:** BR-01, BR-03, FR-02  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-03.1:** Ein berechtigter Benutzer kann einen bestehenden Kundendatensatz öffnen und bearbeiten.
- **AC-03.2:** Das System übernimmt gültige Änderungen nach erfolgreicher Speicherung.
- **AC-03.3:** Bei fehlenden Berechtigungen verhindert das System die Speicherung der Änderung.

### US-04: Kundeninformationen suchen

**User Story**

Als Vertriebsmitarbeiter möchte ich Kunden anhand definierter Suchkriterien finden können, damit ich relevante Kundeninformationen schnell aufrufen kann.

**Zugehörige Anforderungen:** BR-03, BR-04, FR-04  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-04.1:** Der Benutzer kann die vereinbarten Suchkriterien eingeben.
- **AC-04.2:** Das System zeigt die passenden Kundendatensätze an, auf die der Benutzer zugreifen darf.
- **AC-04.3:** Wenn keine passenden Datensätze gefunden werden, zeigt das System einen entsprechenden Hinweis an.

### US-05: Kundenkontakt dokumentieren

**User Story**

Als Vertriebsmitarbeiter möchte ich Kundenkontakte im CRM dokumentieren können, damit relevante Interaktionen für berechtigte Mitarbeitende nachvollziehbar bleiben.

**Zugehörige Anforderungen:** BR-02, BR-03, FR-05  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-05.1:** Der Benutzer kann eine Kundenaktivität mit den fachlich erforderlichen Angaben erfassen.
- **AC-05.2:** Die Aktivität wird einem bestehenden Kundendatensatz zugeordnet.
- **AC-05.3:** Nach erfolgreicher Speicherung ist die Aktivität am zugehörigen Kundendatensatz für berechtigte Benutzer nachvollziehbar.

### US-06: Vertriebschance verwalten

**User Story**

Als Vertriebsmitarbeiter möchte ich Vertriebschancen anlegen und aktualisieren können, damit ich laufende Verkaufsaktivitäten strukturiert nachverfolgen kann.

**Zugehörige Anforderungen:** BR-02, BR-04, FR-06  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-06.1:** Ein berechtigter Benutzer kann eine Vertriebschance mit den festgelegten Pflichtangaben anlegen.
- **AC-06.2:** Eine Vertriebschance kann einem bestehenden Kunden zugeordnet werden.
- **AC-06.3:** Der Benutzer kann die gespeicherten Angaben einer Vertriebschance aktualisieren.

### US-07: Status einer Vertriebschance aktualisieren

**User Story**

Als Vertriebsmitarbeiter möchte ich den Status einer Vertriebschance aktualisieren können, damit der aktuelle Bearbeitungsstand im CRM nachvollziehbar ist.

**Zugehörige Anforderungen:** BR-02, FR-07  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-07.1:** Der Benutzer kann einen Status aus der fachlich festgelegten Auswahl auswählen.
- **AC-07.2:** Das System speichert einen zulässigen Statuswechsel.
- **AC-07.3:** Der aktualisierte Status wird in der Vertriebschancenübersicht angezeigt.

### US-08: Vertriebschancenübersicht einsehen

**User Story**

Als Vertriebsleiter möchte ich eine Übersicht der Vertriebschancen und ihrer aktuellen Status einsehen können, damit ich laufende Vertriebsaktivitäten besser überblicken kann.

**Zugehörige Anforderungen:** BR-02, FR-08  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-08.1:** Die Übersicht zeigt mindestens die Vertriebschance, den zugehörigen Kunden und den aktuellen Status.
- **AC-08.2:** Der Benutzer kann die Übersicht anhand der vereinbarten Kriterien filtern.
- **AC-08.3:** Es werden ausschließlich Vertriebschancen angezeigt, auf die der Benutzer zugreifen darf.

### US-09: Benutzerberechtigungen verwalten

**User Story**

Als CRM-Administrator möchte ich Benutzerrollen und Berechtigungen verwalten können, damit der Zugriff auf Kunden- und Vertriebsinformationen kontrolliert erfolgt.

**Zugehörige Anforderungen:** BR-05, FR-09  
**Priorität:** Hoch

**Akzeptanzkriterien**

- **AC-09.1:** Ein entsprechend berechtigter Administrator kann die vorgesehenen Benutzerrollen verwalten.
- **AC-09.2:** Berechtigungen können den definierten Rollen zugeordnet werden.
- **AC-09.3:** Benutzer ohne die erforderlichen Rechte können keine geschützten Funktionen ausführen.

**Offener Punkt:** Die konkreten Rollen, Berechtigungen und Verwaltungsregeln müssen festgelegt werden.

## 3. Priorisierungsübersicht

| ID | User Story | Priorität | Fachlicher Schwerpunkt |
|---|---|---|---|
| US-01 | Kundendatensatz anlegen | Hoch | Kundendatenpflege |
| US-02 | Mögliche Dubletten erkennen | Hoch | Datenqualität |
| US-03 | Kundendaten bearbeiten | Hoch | Datenpflege |
| US-04 | Kundeninformationen suchen | Hoch | Informationszugriff |
| US-05 | Kundenkontakt dokumentieren | Hoch | Nachvollziehbarkeit |
| US-06 | Vertriebschance verwalten | Hoch | Vertriebsprozess |
| US-07 | Status aktualisieren | Hoch | Statusverwaltung |
| US-08 | Vertriebschancenübersicht einsehen | Hoch | Transparenz |
| US-09 | Benutzerberechtigungen verwalten | Hoch | Zugriffskontrolle |

## 4. Hinweise zur weiteren Bearbeitung

Die User Stories bilden einen ersten Vorschlag für ein Product Backlog. Vor einer tatsächlichen Umsetzung sollten sie mit den Stakeholdern validiert, hinsichtlich ihrer Größe und Abhängigkeiten überprüft und priorisiert werden.

Die Akzeptanzkriterien dienen als Grundlage für die spätere fachliche Abnahme und die Ableitung von Testfällen.