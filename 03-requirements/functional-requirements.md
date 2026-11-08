# Functional Requirements – CRM-Modernisierung

## 1. Ziel

Dieses Dokument beschreibt die funktionalen Anforderungen an die geplante CRM-Lösung.

Die Anforderungen leiten sich aus den Business Requirements ab und definieren konkrete Funktionen, die das System bereitstellen soll. Da es sich um eine fiktive Fallstudie handelt, sind die Anforderungen zunächst fachliche Vorschläge und noch nicht durch reale Stakeholder validiert.

## 2. Funktionale Anforderungen

### FR-01: Kundendatensätze anlegen

**Beschreibung:**
Das System muss berechtigten Mitarbeitenden ermöglichen, neue Kundendatensätze anzulegen.

**Zugehörige Business Requirements:** BR-01, BR-03

**Akzeptanzkriterien:**

* Ein berechtigter Benutzer kann einen neuen Kundendatensatz erstellen.
* Pflichtfelder müssen vor dem Speichern ausgefüllt sein.
* Bei fehlenden Pflichtangaben zeigt das System eine verständliche Fehlermeldung an.

**Priorität:** Hoch

### FR-02: Kundendaten bearbeiten

**Beschreibung:**
Das System muss berechtigten Mitarbeitenden ermöglichen, bestehende Kundendatensätze zu bearbeiten.

**Zugehörige Business Requirements:** BR-01, BR-03

**Akzeptanzkriterien:**

* Ein berechtigter Benutzer kann vorhandene Kundendaten ändern.
* Änderungen werden nach erfolgreicher Speicherung im Datensatz angezeigt.
* Nicht berechtigte Benutzer können keine Änderungen speichern.

**Priorität:** Hoch

### FR-03: Mögliche Dubletten erkennen

**Beschreibung:**
Das System soll beim Anlegen eines Kundendatensatzes auf mögliche Dubletten hinweisen.

**Zugehörige Business Requirements:** BR-01

**Akzeptanzkriterien:**

* Vor dem Speichern prüft das System definierte Identifikationsmerkmale auf mögliche Übereinstimmungen.
* Bei einem möglichen Treffer zeigt das System einen Hinweis mit den relevanten Vergleichsinformationen an.
* Der Benutzer kann den bestehenden Datensatz prüfen, bevor er fortfährt.

**Offene Klärung:**
Die zu verwendenden Identifikationsmerkmale und die Regeln zur Dublettenerkennung müssen fachlich festgelegt werden.

**Priorität:** Hoch

### FR-04: Kundeninformationen suchen

**Beschreibung:**
Das System muss berechtigten Mitarbeitenden ermöglichen, Kunden anhand definierter Suchkriterien zu finden.

**Zugehörige Business Requirements:** BR-03, BR-04

**Akzeptanzkriterien:**

* Benutzer können nach festgelegten Kundenmerkmalen suchen.
* Die Suchergebnisse zeigen die wesentlichen Informationen zur Identifikation eines Kunden.
* Benutzer können einen Suchtreffer öffnen, sofern sie über die erforderlichen Berechtigungen verfügen.

**Offene Klärung:**
Die unterstützten Suchfelder und Filter müssen festgelegt werden.

**Priorität:** Hoch

### FR-05: Kundenkontakte dokumentieren

**Beschreibung:**
Das System muss ermöglichen, Kundenkontakte und zugehörige Aktivitäten einem Kundendatensatz zuzuordnen.

**Zugehörige Business Requirements:** BR-02, BR-03

**Akzeptanzkriterien:**

* Ein berechtigter Benutzer kann eine Kundenaktivität erfassen.
* Eine Aktivität wird einem Kunden zugeordnet.
* Die dokumentierte Aktivität ist für berechtigte Benutzer am zugehörigen Kundendatensatz nachvollziehbar.

**Offene Klärung:**
Die erforderlichen Aktivitätstypen und Pflichtfelder müssen festgelegt werden.

**Priorität:** Hoch

### FR-06: Vertriebschancen verwalten

**Beschreibung:**
Das System muss ermöglichen, Vertriebschancen anzulegen und ihre relevanten Informationen zu pflegen.

**Zugehörige Business Requirements:** BR-02, BR-04

**Akzeptanzkriterien:**

* Berechtigte Benutzer können eine Vertriebschance anlegen.
* Eine Vertriebschance kann einem Kunden zugeordnet werden.
* Relevante Angaben zur Vertriebschance können gespeichert und aktualisiert werden.

**Offene Klärung:**
Pflichtfelder und Statuswerte für Vertriebschancen müssen fachlich definiert werden.

**Priorität:** Hoch

### FR-07: Status von Vertriebschancen aktualisieren

**Beschreibung:**
Das System muss berechtigten Benutzern ermöglichen, den Bearbeitungsstatus einer Vertriebschance zu aktualisieren.

**Zugehörige Business Requirements:** BR-02

**Akzeptanzkriterien:**

* Der Benutzer kann den Status aus einer festgelegten Auswahl auswählen.
* Das System speichert den neuen Status.
* Der aktuelle Status ist in der Übersicht der Vertriebschancen sichtbar.

**Offene Klärung:**
Die Statuswerte und zulässigen Statusübergänge müssen festgelegt werden.

**Priorität:** Hoch

### FR-08: Vertriebschancen übersichtlich anzeigen

**Beschreibung:**
Das System muss eine Übersicht über Vertriebschancen bereitstellen, auf die der jeweilige Benutzer zugreifen darf.

**Zugehörige Business Requirements:** BR-02

**Akzeptanzkriterien:**

* Die Übersicht zeigt mindestens den Namen der Vertriebschance, den zugehörigen Kunden und den aktuellen Status.
* Benutzer können die Übersicht nach festgelegten Kriterien filtern.
* Es werden nur Vertriebschancen angezeigt, für die der Benutzer eine entsprechende Berechtigung besitzt.

**Offene Klärung:**
Zusätzliche Spalten und Filter müssen mit den Stakeholdern abgestimmt werden.

**Priorität:** Hoch

### FR-09: Zugriffe rollenbasiert kontrollieren

**Beschreibung:**
Das System muss Zugriffe auf Kundendaten und Vertriebsinformationen entsprechend den festgelegten Benutzerrollen und Berechtigungen kontrollieren.

**Zugehörige Business Requirements:** BR-05

**Akzeptanzkriterien:**

* Benutzer können nur auf Funktionen und Daten zugreifen, für die sie berechtigt sind.
* Nicht erlaubte Zugriffsversuche werden verhindert.
* Die Berechtigungen können einer definierten Benutzerrolle zugeordnet werden.

**Offene Klärung:**
Das konkrete Rollen- und Berechtigungsmodell muss abgestimmt werden.

**Priorität:** Hoch

## 3. Übersicht und Rückverfolgbarkeit

| ID    | Funktion                                  | Zugehörige Business Requirements | Priorität |
| ----- | ----------------------------------------- | -------------------------------- | --------- |
| FR-01 | Kundendatensätze anlegen                  | BR-01, BR-03                     | Hoch      |
| FR-02 | Kundendaten bearbeiten                    | BR-01, BR-03                     | Hoch      |
| FR-03 | Mögliche Dubletten erkennen               | BR-01                            | Hoch      |
| FR-04 | Kundeninformationen suchen                | BR-03, BR-04                     | Hoch      |
| FR-05 | Kundenkontakte dokumentieren              | BR-02, BR-03                     | Hoch      |
| FR-06 | Vertriebschancen verwalten                | BR-02, BR-04                     | Hoch      |
| FR-07 | Status von Vertriebschancen aktualisieren | BR-02                            | Hoch      |
| FR-08 | Vertriebschancen übersichtlich anzeigen   | BR-02                            | Hoch      |
| FR-09 | Zugriffe rollenbasiert kontrollieren      | BR-05                            | Hoch      |

## 4. Offene fachliche Fragen

Vor einer detaillierten Ausarbeitung müssen insbesondere folgende Punkte geklärt werden:

1. Welche Felder sind für Kunden und Vertriebschancen verpflichtend?
2. Nach welchen Kriterien werden mögliche Dubletten erkannt?
3. Welche Aktivitätstypen müssen dokumentiert werden?
4. Welche Statuswerte und Statusübergänge gelten für Vertriebschancen?
5. Welche Benutzerrollen und Berechtigungen werden benötigt?
6. Welche Such- und Filtermöglichkeiten sind erforderlich?

## 5. Hinweis zur Validierung

Die Anforderungen sind ein erster fachlicher Entwurf. In einem realen Projekt müssten sie mit den relevanten Stakeholdern abgestimmt, hinsichtlich ihrer Machbarkeit geprüft und anschließend verbindlich priorisiert werden.
