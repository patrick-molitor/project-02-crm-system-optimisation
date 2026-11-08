# Requirements Traceability Matrix (RTM)

## 1. Ziel

Diese Matrix dokumentiert die Beziehungen zwischen den Business Requirements (BRs), Functional Requirements (FRs) und Non-Functional Requirements (NFRs).

Sie unterstützt die Rückverfolgbarkeit der Anforderungen und hilft dabei, Lücken, Abhängigkeiten und mögliche Auswirkungen von Änderungen zu erkennen.

Da es sich um eine fiktive Fallstudie handelt, bilden die Zuordnungen einen fachlichen Entwurf und müssen in einem realen Projekt mit den Stakeholdern validiert werden.

## 2. Rückverfolgbarkeit: Business Requirements zu Functional Requirements

| Business Requirement | Zugeordnete Functional Requirements |
|---|---|
| BR-01: Einheitliche Kundendatenpflege | FR-01, FR-02, FR-03 |
| BR-02: Transparenz über Vertriebschancen | FR-06, FR-07, FR-08 |
| BR-03: Zentraler Zugriff auf Kundeninformationen | FR-01, FR-02, FR-04, FR-05 |
| BR-04: Effizientere Vertriebsabläufe | FR-04, FR-06 |
| BR-05: Datenschutz und kontrollierter Datenzugriff | FR-09 |

## 3. Rückverfolgbarkeit: Business Requirements zu Non-Functional Requirements

| Business Requirement | Zugeordnete Non-Functional Requirements |
|---|---|
| BR-01: Einheitliche Kundendatenpflege | NFR-02, NFR-05 |
| BR-02: Transparenz über Vertriebschancen | NFR-04, NFR-05 |
| BR-03: Zentraler Zugriff auf Kundeninformationen | NFR-01, NFR-03, NFR-04, NFR-05 |
| BR-04: Effizientere Vertriebsabläufe | NFR-01, NFR-02, NFR-04 |
| BR-05: Datenschutz und kontrollierter Datenzugriff | NFR-03 |

## 4. Übersicht der Anforderungsbeziehungen

| Anforderung | Zugeordnete Business Requirements | Zugeordnete weitere Anforderungen |
|---|---|---|
| FR-01 | BR-01, BR-03 | NFR-02, NFR-05 |
| FR-02 | BR-01, BR-03 | NFR-02, NFR-05 |
| FR-03 | BR-01 | NFR-05 |
| FR-04 | BR-03, BR-04 | NFR-01, NFR-02 |
| FR-05 | BR-03 | NFR-03, NFR-05 |
| FR-06 | BR-02, BR-04 | NFR-02, NFR-05 |
| FR-07 | BR-02 | NFR-05 |
| FR-08 | BR-02 | NFR-01, NFR-03, NFR-04 |
| FR-09 | BR-05 | NFR-03 |

## 5. Anforderungen ohne direkte Zuordnung

NFR-06 (Wartbarkeit) besitzt aktuell keine direkte Zuordnung zu einer Business Requirement.

Die Anforderung beschreibt ein technisches Qualitätsmerkmal, das den langfristigen Betrieb und die Weiterentwicklung der CRM-Lösung unterstützt.

Eine direkte geschäftliche Zuordnung müsste durch zusätzliche fachliche Ziele oder Stakeholderbedürfnisse begründet werden.

## 6. Änderungsmanagement

Änderungen an Anforderungen sollen hinsichtlich ihrer Auswirkungen auf verknüpfte Anforderungen überprüft werden.

Beispielsweise könnte eine Änderung am Rollen- und Berechtigungskonzept FR-09 und NFR-03 betreffen.

Eine Änderung an der Kundendatenpflege könnte Auswirkungen auf FR-01, FR-02, FR-03 sowie NFR-02 und NFR-05 haben.

## 7. Grenzen der Matrix

Die Matrix dokumentiert die Beziehungen zwischen Business Requirements, Functional Requirements und Non-Functional Requirements.

Eine vollständige Rückverfolgbarkeit würde zusätzlich die Verbindung zu Stakeholderbedürfnissen, Use Cases, User Stories, Akzeptanzkriterien und späteren Testfällen berücksichtigen.

Die Zuordnungen stellen einen fachlichen Entwurf dar und müssen im Rahmen einer realen Projektvalidierung bestätigt werden.