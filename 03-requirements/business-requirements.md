# Business Requirements – CRM-Modernisierung

## 1. Ziel

Dieses Dokument beschreibt die geschäftlichen Anforderungen an die Modernisierung der CRM-Unterstützung eines fiktiven mittelständischen B2B-Unternehmens.

Die Business Requirements leiten sich aus der angenommenen Problemstellung und der Stakeholderanalyse ab. Sie beschreiben die gewünschten Geschäftsergebnisse, ohne bereits konkrete technische Lösungen vorzugeben.

## 2. Business Requirements

### BR-01: Einheitliche Kundendatenpflege

**Beschreibung:**
Das Unternehmen benötigt einen einheitlichen Ansatz zur Pflege von Kundeninformationen, um uneinheitliche Datenbestände und unnötige Doppeleingaben zu reduzieren.

**Begründung:**
Uneinheitliche Datenpflege erschwert die Nutzung und Weitergabe von Kundeninformationen.

**Erwarteter Nutzen:**
Verbesserte Datenkonsistenz und effizientere Arbeitsabläufe.

**Priorität:** Hoch

### BR-02: Verbesserte Transparenz über Vertriebschancen

**Beschreibung:**
Das Unternehmen benötigt eine nachvollziehbare Übersicht über Vertriebschancen und deren Bearbeitungsstatus.

**Begründung:**
Eine eingeschränkte Übersicht erschwert die Steuerung und Nachverfolgung von Vertriebsaktivitäten.

**Erwarteter Nutzen:**
Bessere Übersicht über laufende Vertriebsaktivitäten und deren Status.

**Priorität:** Hoch

### BR-03: Zentraler Zugriff auf Kundeninformationen

**Beschreibung:**
Relevante Kundeninformationen und Kontaktaktivitäten sollen für berechtigte Mitarbeitende nachvollziehbar und zentral verfügbar sein.

**Begründung:**
Verteilte oder nicht aktuelle Informationen erschweren die Zusammenarbeit und können zu Informationsverlusten führen.

**Erwarteter Nutzen:**
Bessere Informationsverfügbarkeit und erleichterte Übergaben zwischen Mitarbeitenden.

**Priorität:** Hoch

### BR-04: Effizientere Vertriebsabläufe

**Beschreibung:**
Der Aufwand für wiederkehrende administrative Tätigkeiten im Zusammenhang mit Kundeninformationen und Vertriebsaktivitäten soll reduziert werden.

**Begründung:**
Manuelle und doppelte Arbeit bindet Zeit, die für vertriebliche Aufgaben eingesetzt werden könnte.

**Erwarteter Nutzen:**
Weniger vermeidbarer Verwaltungsaufwand.

**Priorität:** Mittel

### BR-05: Datenschutz und kontrollierter Datenzugriff

**Beschreibung:**
Die CRM-Lösung muss die angemessene Verarbeitung personenbezogener Daten und eine rollenbezogene Kontrolle des Datenzugriffs unterstützen.

**Begründung:**
Kundeninformationen können personenbezogene und vertrauliche Daten enthalten.

**Erwarteter Nutzen:**
Unterstützung eines verantwortungsvollen und regelkonformen Umgangs mit Daten.

**Priorität:** Hoch

## 3. Priorisierungsübersicht

| ID    | Business Requirement                        | Priorität | Primär betroffene Stakeholder            |
| ----- | ------------------------------------------- | --------- | ---------------------------------------- |
| BR-01 | Einheitliche Kundendatenpflege              | Hoch      | Vertriebsmitarbeitende, Vertriebsleitung |
| BR-02 | Transparenz über Vertriebschancen           | Hoch      | Vertriebsleitung, Vertriebsmitarbeitende |
| BR-03 | Zentraler Zugriff auf Kundeninformationen   | Hoch      | Vertriebsmitarbeitende, IT               |
| BR-04 | Effizientere Vertriebsabläufe               | Mittel    | Vertriebsmitarbeitende, Geschäftsführung |
| BR-05 | Datenschutz und kontrollierter Datenzugriff | Hoch      | Datenschutzverantwortliche, IT           |

## 4. Annahmen und offene Fragen

Die Anforderungen basieren auf dem fiktiven Ausgangsszenario und wurden noch nicht durch reale Stakeholder bestätigt.

Für eine spätere Konkretisierung sind insbesondere folgende Fragen zu klären:

* Welche Kundendaten müssen verpflichtend gepflegt werden?
* Wie sollen doppelte Kundendatensätze erkannt und behandelt werden?
* Welche Status benötigt eine Vertriebschance?
* Welche Informationen müssen bei einer Übergabe zwischen Mitarbeitenden verfügbar sein?
* Welche Rollen dürfen welche Daten einsehen oder verändern?
* An welchen Kennzahlen lässt sich eine Verbesserung der Vertriebsabläufe messen?

## 5. Abgrenzung zu funktionalen Anforderungen

Die Business Requirements beschreiben die gewünschten Geschäftsergebnisse. Sie legen noch nicht fest, welche konkreten Funktionen das CRM-System dafür bereitstellen muss.

Im nächsten Schritt werden daraus funktionale und nichtfunktionale Anforderungen abgeleitet. Diese werden mit eindeutigen IDs dokumentiert und den jeweiligen Business Requirements zugeordnet.
