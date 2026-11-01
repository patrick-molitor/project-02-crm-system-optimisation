# Non-Functional Requirements (NFRs) – CRM-Modernisierung

## 1. Ziel und Kontext

Dieses Dokument beschreibt die nichtfunktionalen Anforderungen an die geplante CRM-Lösung eines fiktiven mittelständischen B2B-Unternehmens.

Die Anforderungen ergänzen die Business Requirements (BRs) und Functional Requirements (FRs). Sie beschreiben Qualitätsmerkmale und Rahmenbedingungen, unter denen die CRM-Lösung genutzt und betrieben werden soll.

Da es sich um eine fiktive Fallstudie handelt, sind die Anforderungen zunächst Vorschläge. Die Zielwerte und Rahmenbedingungen müssen vor einer tatsächlichen Umsetzung mit den relevanten Stakeholdern abgestimmt werden.

## 2. Nichtfunktionale Anforderungen

### NFR-01: Antwortzeit

**Beschreibung:**
Die CRM-Lösung soll bei typischen Benutzeraktionen eine angemessene Antwortzeit gewährleisten.

**Akzeptanzkriterium:**
Bei einer definierten Referenzlast werden mindestens 95 % der Suchanfragen innerhalb von 2 Sekunden beantwortet.

**Begründung:**
Kurze Antwortzeiten unterstützen effiziente Arbeitsabläufe im Vertrieb.

**Zugehörige Anforderungen:** BR-03, BR-04; FR-04

**Priorität:** Hoch

**Offene Klärung:**
Die Referenzlast, die Testumgebung und die genaue Definition einer Suchanfrage müssen festgelegt werden.

### NFR-02: Benutzbarkeit

**Beschreibung:**
Die CRM-Lösung soll typische Aufgaben der Kundendatenpflege und Vertriebsverwaltung verständlich und mit möglichst geringem Bedienaufwand unterstützen.

**Akzeptanzkriterium:**
Mindestens 90 % einer definierten Gruppe repräsentativer Testpersonen können die vereinbarten Kernaufgaben ohne Unterstützung erfolgreich abschließen.

**Begründung:**
Eine verständliche Bedienung kann Einarbeitungsaufwand und Bedienfehler reduzieren.

**Zugehörige Anforderungen:** BR-01, BR-04; FR-01, FR-02, FR-04, FR-06

**Priorität:** Hoch

**Offene Klärung:**
Die Kernaufgaben, die Zusammensetzung der Testgruppe und die Bedingungen des Usability-Tests müssen festgelegt werden.

### NFR-03: Zugriffssicherheit

**Beschreibung:**
Die CRM-Lösung muss Informationen und Funktionen vor unberechtigtem Zugriff schützen.

**Akzeptanzkriterium:**
Alle in einem abgestimmten Berechtigungstest definierten unberechtigten Zugriffsversuche auf geschützte Funktionen und Daten werden verhindert.

**Begründung:**
Kunden- und Vertriebsinformationen können vertrauliche oder personenbezogene Daten enthalten.

**Zugehörige Anforderungen:** BR-05; FR-09

**Priorität:** Hoch

**Offene Klärung:**
Das Rollenmodell, die Schutzbedarfe der Daten und die konkreten Testfälle müssen abgestimmt werden.

### NFR-04: Verfügbarkeit

**Beschreibung:**
Die CRM-Lösung soll während der vereinbarten Geschäftszeiten für berechtigte Benutzer verfügbar sein.

**Akzeptanzkriterium:**
Die monatliche Verfügbarkeit beträgt mindestens 99,5 % innerhalb der vereinbarten Servicezeiten. Geplante Wartungsfenster werden nach einer festgelegten Regel behandelt.

**Begründung:**
Die Verfügbarkeit des Systems unterstützt die kontinuierliche Bearbeitung von Kundenkontakten und Vertriebschancen.

**Zugehörige Anforderungen:** BR-02, BR-03, BR-04

**Priorität:** Mittel

**Offene Klärung:**
Servicezeiten, Messverfahren, zulässige Wartungsfenster und Ausnahmen müssen definiert werden.

### NFR-05: Datenintegrität

**Beschreibung:**
Die CRM-Lösung muss die Konsistenz und Vollständigkeit gespeicherter Kunden- und Vertriebsdaten unterstützen.

**Akzeptanzkriterium:**
In den definierten Integritätstests werden alle festgelegten Datenregeln eingehalten. Ungültige oder unzulässige Datenänderungen werden entsprechend den fachlichen Regeln verhindert.

**Begründung:**
Konsistente Daten sind eine Grundlage für zuverlässige Kundeninformationen und aussagekräftige Vertriebsübersichten.

**Zugehörige Anforderungen:** BR-01, BR-02, BR-03; FR-01, FR-02, FR-06, FR-07

**Priorität:** Hoch

**Offene Klärung:**
Die fachlichen Datenregeln und die zugehörigen Testfälle müssen spezifiziert werden.

### NFR-06: Wartbarkeit

**Beschreibung:**
Die CRM-Lösung soll so gestaltet und dokumentiert sein, dass Änderungen und Fehlerbehebungen mit nachvollziehbarem Aufwand durchgeführt werden können.

**Akzeptanzkriterium:**
Für die vereinbarten Kernkomponenten liegen aktuelle technische Dokumentationen vor. Ein definierter Änderungstest kann anhand der Dokumentation nachvollzogen und durchgeführt werden.

**Begründung:**
Eine wartbare Lösung erleichtert den langfristigen Betrieb und die Weiterentwicklung.

**Zugehörige Anforderungen:** BR-01 bis BR-05

**Priorität:** Mittel

**Offene Klärung:**
Dokumentationsumfang, technische Standards und der Ablauf des Änderungstests müssen festgelegt werden.

## 3. Übersicht

| ID     | Qualitätsmerkmal   | Messbares Kriterium                                                           | Priorität |
| ------ | ------------------ | ----------------------------------------------------------------------------- | --------- |
| NFR-01 | Antwortzeit        | 95 % der Suchanfragen innerhalb von 2 Sekunden                                | Hoch      |
| NFR-02 | Benutzbarkeit      | 90 % der Testpersonen schließen definierte Kernaufgaben ohne Unterstützung ab | Hoch      |
| NFR-03 | Zugriffssicherheit | Alle definierten unberechtigten Zugriffsversuche werden verhindert            | Hoch      |
| NFR-04 | Verfügbarkeit      | Mindestens 99,5 % innerhalb der vereinbarten Servicezeiten                    | Mittel    |
| NFR-05 | Datenintegrität    | Alle definierten Integritätsregeln werden in den Tests eingehalten            | Hoch      |
| NFR-06 | Wartbarkeit        | Dokumentierte Kernkomponenten und nachvollziehbarer Änderungstest             | Mittel    |

## 4. Hinweise zur Bewertung

Die angegebenen Zielwerte sind beispielhafte Ausgangswerte für diese Fallstudie. Sie sind keine bestätigten Geschäftsanforderungen und stellen keine Aussage über die Leistungsfähigkeit eines bestehenden Systems dar.

Vor einer Umsetzung müssen die Anforderungen auf ihre Angemessenheit, Messbarkeit, technische Machbarkeit und Wirtschaftlichkeit geprüft werden.

Insbesondere müssen die Messbedingungen so festgelegt werden, dass die Akzeptanzkriterien eindeutig überprüfbar sind.

## 5. Abgrenzung zu funktionalen Anforderungen

Funktionale Anforderungen beschreiben, welche Funktionen das System bereitstellen muss. Nichtfunktionale Anforderungen beschreiben hier vor allem, welche Qualitätsmerkmale diese Lösung erfüllen soll.

Die Unterscheidung richtet sich nach dem konkreten Inhalt der Anforderung. Beispielsweise beschreibt FR-09 eine konkrete Funktion zur Zugriffskontrolle, während NFR-03 das angestrebte Sicherheitsniveau und dessen Überprüfung konkretisiert.
