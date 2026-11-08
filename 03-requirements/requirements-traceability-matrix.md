# Requirements Traceability Matrix (RTM)

## 1. Ziel

Diese Matrix dokumentiert die Beziehungen zwischen den Business Requirements (BRs), Functional Requirements (FRs) und Non-Functional Requirements (NFRs).

Sie unterstützt die Rückverfolgbarkeit der Anforderungen und hilft dabei, Lücken, Abhängigkeiten und mögliche Auswirkungen von Änderungen zu erkennen.

Da die Fallstudie fiktiv ist, bilden die Zuordnungen einen fachlichen Entwurf und müssen in einem realen Projekt mit den Stakeholdern validiert werden.

## 2. Rückverfolgbarkeitsmatrix

| Business Requirement                               | Zugeordnete Functional Requirements | Zugeordnete Non-Functional Requirements |
| -------------------------------------------------- | ----------------------------------- | --------------------------------------- |
| BR-01: Einheitliche Kundendatenpflege              | FR-01, FR-02, FR-03                 | NFR-02, NFR-05, NFR-06                  |
| BR-02: Transparenz über Vertriebschancen           | FR-05, FR-06, FR-07, FR-08          | NFR-01, NFR-04, NFR-05                  |
| BR-03: Zentraler Zugriff auf Kundeninformationen   | FR-01, FR-02, FR-04, FR-05          | NFR-01, NFR-03, NFR-04, NFR-05          |
| BR-04: Effizientere Vertriebsabläufe               | FR-04, FR-06                        | NFR-01, NFR-02, NFR-06                  |
| BR-05: Datenschutz und kontrollierter Datenzugriff | FR-09                               | NFR-03, NFR-05                          |

## 3. Anforderungen ohne direkte Zuordnung

Die folgenden Punkte müssen bei der weiteren Bearbeitung überprüft werden:

* Ob alle FRs ausreichend durch mindestens eine Business Requirement begründet sind.
* Ob alle NFRs einen klaren Bezug zu den Geschäftszielen besitzen.
* Ob die Zuordnungen zwischen den Anforderungen fachlich korrekt und vollständig sind.
* Ob zusätzliche Anforderungen aus den Use Cases oder Stakeholderbedürfnissen entstehen.

## 4. Änderungsmanagement

Änderungen an Anforderungen sollen hinsichtlich ihrer Auswirkungen auf verknüpfte Anforderungen überprüft werden.

Beispielsweise könnte eine Änderung am Rollen- und Berechtigungskonzept FR-09 und NFR-03 betreffen. Je nach Umfang könnte dies auch Auswirkungen auf die Anforderungen an die Datenintegrität oder auf weitere fachliche Abläufe haben.

## 5. Grenzen der Matrix

Die Matrix dokumentiert derzeit vor allem Beziehungen zwischen Business Requirements, Functional Requirements und Non-Functional Requirements.

Eine vollständige Rückverfolgbarkeit würde zusätzlich die Verbindung zu Stakeholderbedürfnissen, Use Cases, Akzeptanzkriterien und späteren Testfällen berücksichtigen.
