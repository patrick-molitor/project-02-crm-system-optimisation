# Non-Functional Requirements (NFRs) – CRM-Modernisierung

## 1. Ziel und Kontext

Dieses Dokument beschreibt die nichtfunktionalen Anforderungen an die geplante CRM-Lösung eines fiktiven mittelständischen B2B-Unternehmens.

Die Anforderungen ergänzen die Business Requirements (BRs) und Functional Requirements (FRs). Sie beschreiben Qualitätsmerkmale und Rahmenbedingungen, unter denen die CRM-Lösung genutzt und betrieben werden soll.

Da es sich um eine fiktive Fallstudie handelt, sind die Anforderungen und Zielwerte beispielhafte Vorschläge. Sie müssen vor einer tatsächlichen Umsetzung mit den relevanten Stakeholdern abgestimmt werden.

## 2. Nichtfunktionale Anforderungen

### NFR-01: Antwortzeit

**Beschreibung:**

Die CRM-Lösung soll bei typischen Benutzeraktionen eine angemessene Antwortzeit gewährleisten.

**Akzeptanzkriterien:**

- Mindestens 95 % der Suchanfragen werden innerhalb von 2 Sekunden beantwortet.
- Die Messung erfolgt unter einer zuvor definierten Referenzlast.
- Die Antwortzeit wird vom Absenden der Suchanfrage bis zur vollständigen Anzeige der Suchergebnisse gemessen.

**Begründung:**

Kurze Antwortzeiten unterstützen effiziente Arbeitsabläufe im Vertrieb.

**Zugehörige Anforderungen:** BR-03, BR-04; FR-04, FR-08

**Priorität:** Hoch

**Offene Klärung:**

Die Referenzlast, die Testumgebung und die Anzahl gleichzeitiger Benutzer müssen festgelegt werden.

### NFR-02: Benutzbarkeit

**Beschreibung:**

Die CRM-Lösung soll typische Aufgaben der Kundendatenpflege und Vertriebsverwaltung verständlich und mit möglichst geringem Bedienaufwand unterstützen.

**Akzeptanzkriterien:**

- Mindestens 90 % einer definierten Gruppe repräsentativer Testpersonen können die vereinbarten Kernaufgaben ohne Unterstützung erfolgreich abschließen.
- Die Testpersonen erhalten vor dem Test eine einheitliche Einführung.
- Die Ergebnisse werden anhand einer vorher festgelegten Aufgabenliste dokumentiert.

**Begründung:**

Eine verständliche Bedienung kann Einarbeitungsaufwand und Bedienfehler reduzieren.

**Zugehörige Anforderungen:** BR-01, BR-04; FR-01, FR-02, FR-04, FR-06

**Priorität:** Hoch

**Offene Klärung:**

Die Kernaufgaben, die Zusammensetzung der Testgruppe und die Bedingungen des Usability-Tests müssen festgelegt werden.

### NFR-03: Zugriffssicherheit

**Beschreibung:**

Die CRM-Lösung muss Informationen und Funktionen vor unberechtigtem Zugriff schützen.

**Akzeptanzkriterien:**

- Alle im abgestimmten Berechtigungstest definierten unberechtigten Zugriffsversuche werden verhindert.
- Benutzer können ausschließlich auf Funktionen und Daten zugreifen, für die sie eine entsprechende Berechtigung besitzen.
- Berechtigungsprüfungen werden sowohl beim Aufruf geschützter Funktionen als auch bei entsprechenden Datenzugriffen berücksichtigt.

**Begründung:**

Kunden- und Vertriebsinformationen können vertrauliche oder personenbezogene Daten enthalten.

**Zugehörige Anforderungen:** BR-05; FR-09

**Priorität:** Hoch

**Offene Klärung:**

Das Rollenmodell, die Schutzbedarfe der Daten und die konkreten Testfälle müssen abgestimmt werden.

### NFR-04: Verfügbarkeit

**Beschreibung:**

Die CRM-Lösung soll während der vereinbarten Geschäftszeiten für berechtigte Benutzer verfügbar sein.

**Akzeptanzkriterien:**

- Die monatliche Verfügbarkeit beträgt mindestens 99,5 % innerhalb der vereinbarten Servicezeiten.
- Die Verfügbarkeit wird anhand der vereinbarten Messmethode ermittelt.
- Geplante Wartungsfenster werden entsprechend einer festgelegten Regel behandelt.

**Begründung:**

Die Verfügbarkeit des Systems unterstützt die kontinuierliche Bearbeitung von Kundenkontakten und Vertriebschancen.

**Zugehörige Anforderungen:** BR-02, BR-03, BR-04

**Priorität:** Mittel

**Offene Klärung:**

Servicezeiten, Messverfahren, zulässige Wartungsfenster und Ausnahmen müssen definiert werden.

### NFR-05: Datenintegrität

**Beschreibung:**

Die CRM-Lösung muss die Konsistenz und Vollständigkeit gespeicherter Kunden- und Vertriebsdaten unterstützen.

**Akzeptanzkriterien:**

- Alle definierten fachlichen Datenregeln werden bei der Speicherung und Änderung von Datensätzen eingehalten.
- Ungültige oder unzulässige Datenänderungen werden entsprechend den festgelegten Regeln verhindert.
- Die definierten Integritätstests werden ohne unerwartete Datenabweichungen bestanden.

**Begründung:**

Konsistente Daten sind eine Grundlage für zuverlässige Kundeninformationen und aussagekräftige Vertriebsübersichten.

**Zugehörige Anforderungen:** BR-01, BR-02, BR-03; FR-01, FR-02, FR-03, FR-06, FR-07

**Priorität:** Hoch

**Offene Klärung:**

Die fachlichen Datenregeln und die zugehörigen Testfälle müssen spezifiziert werden.

### NFR-06: Wartbarkeit

**Beschreibung:**

Die CRM-Lösung soll so gestaltet und dokumentiert sein, dass Änderungen und Fehlerbehebungen mit nachvollziehbarem Aufwand durchgeführt werden können.

**Akzeptanzkriterien:**

- Für alle vereinbarten Kernkomponenten liegt eine aktuelle technische Dokumentation vor.
- Änderungen an dokumentierten Kernkomponenten können anhand der vorhandenen Dokumentation nachvollzogen werden.
- Ein definierter Änderungstest kann von einem anderen qualifizierten Teammitglied anhand der Dokumentation durchgeführt werden.

**Begründung:**

Eine wartbare Lösung erleichtert den langfristigen Betrieb und die Weiterentwicklung.

**Zugehörige Anforderungen:** Übergreifendes Qualitätsmerkmal; keine direkte Zuordnung zu einer Business Requirement.

**Priorität:** Mittel

**Offene Klärung:**

Dokumentationsumfang, technische Standards und der Ablauf des Änderungstests müssen festgelegt werden.

## 3. Übersicht

| ID | Qualitätsmerkmal | Akzeptanzkriterium | Priorität |
|---|---|---|---|
| NFR-01 | Antwortzeit | Mindestens 95 % der Suchanfragen innerhalb von 2 Sekunden | Hoch |
| NFR-02 | Benutzbarkeit | Mindestens 90 % der Testpersonen schließen definierte Kernaufgaben ohne Unterstützung ab | Hoch |
| NFR-03 | Zugriffssicherheit | Alle definierten unberechtigten Zugriffsversuche werden verhindert | Hoch |
| NFR-04 | Verfügbarkeit | Mindestens 99,5 % innerhalb der vereinbarten Servicezeiten | Mittel |
| NFR-05 | Datenintegrität | Alle definierten Integritätstests werden bestanden | Hoch |
| NFR-06 | Wartbarkeit | Dokumentierte Kernkomponenten und nachvollziehbarer Änderungstest | Mittel |

## 4. Annahmen und Grenzen

Die angegebenen Zielwerte sind beispielhafte Ausgangswerte für diese Fallstudie. Sie sind keine bestätigten Geschäftsanforderungen und stellen keine Aussage über die Leistungsfähigkeit eines bestehenden Systems dar.

Die Anforderungen müssen vor einer tatsächlichen Umsetzung auf ihre Angemessenheit, Messbarkeit, technische Machbarkeit und Wirtschaftlichkeit geprüft werden.

Insbesondere müssen die Messbedingungen und Testverfahren so festgelegt werden, dass die Akzeptanzkriterien eindeutig überprüfbar sind.

## 5. Abgrenzung zu funktionalen Anforderungen

Funktionale Anforderungen beschreiben, welche Funktionen das System bereitstellen muss.

Nichtfunktionale Anforderungen beschreiben die Qualitätsmerkmale und Rahmenbedingungen, die bei der Bereitstellung dieser Funktionen berücksichtigt werden müssen.

Beispielsweise beschreibt FR-09 eine konkrete Funktion zur Zugriffskontrolle, während NFR-03 das angestrebte Sicherheitsniveau und dessen Überprüfung konkretisiert.