# Use-Case-Übersicht – CRM-Modernisierung

## 1. Ziel

Diese Übersicht identifiziert die wichtigsten Interaktionen zwischen Benutzern und der geplanten CRM-Lösung.

Die Use Cases basieren auf den bisher definierten Business Requirements (BRs), Functional Requirements (FRs) und Non-Functional Requirements (NFRs).

Da es sich um eine fiktive Fallstudie handelt, sind die Use Cases als fachlicher Entwurf zu verstehen.

## 2. Systemgrenze

**System:** CRM-System

Das CRM-System unterstützt die Verwaltung von Kundeninformationen, Kundenkontakten und Vertriebschancen. Es stellt berechtigten Benutzern Funktionen zur Datenpflege und zur Einsicht in relevante Informationen zur Verfügung.

Die nachfolgend beschriebenen Akteure sind externe Rollen, die mit dem System interagieren.

## 3. Akteure

| ID     | Akteur                 | Beschreibung                                                                          |
| ------ | ---------------------- | ------------------------------------------------------------------------------------- |
| ACT-01 | Vertriebsmitarbeitende | Pflegen Kundeninformationen, dokumentieren Kontakte und verwalten Vertriebschancen.   |
| ACT-02 | Vertriebsleitung       | Überwacht Vertriebschancen und nutzt Statusinformationen zur Steuerung des Vertriebs. |
| ACT-03 | CRM-Administration     | Verwaltet Benutzer und Berechtigungen sowie technische Systemeinstellungen.           |

**Hinweis:** Die CRM-Administration ist eine ergänzend angenommene Rolle. Ihre konkreten Verantwortlichkeiten müssen bei einer realen Analyse bestätigt werden.

## 4. Use Cases

| ID    | Use Case                                   | Primärer Akteur        | Zugehörige Anforderungen |
| ----- | ------------------------------------------ | ---------------------- | ------------------------ |
| UC-01 | Kundendatensatz anlegen                    | Vertriebsmitarbeitende | FR-01, FR-03             |
| UC-02 | Kundendaten bearbeiten                     | Vertriebsmitarbeitende | FR-02                    |
| UC-03 | Kundeninformationen suchen                 | Vertriebsmitarbeitende | FR-04                    |
| UC-04 | Kundenkontakt dokumentieren                | Vertriebsmitarbeitende | FR-05                    |
| UC-05 | Vertriebschance anlegen und verwalten      | Vertriebsmitarbeitende | FR-06                    |
| UC-06 | Status einer Vertriebschance aktualisieren | Vertriebsmitarbeitende | FR-07                    |
| UC-07 | Vertriebschancenübersicht einsehen         | Vertriebsleitung       | FR-08                    |
| UC-08 | Benutzerberechtigungen verwalten           | CRM-Administration     | FR-09                    |

## 5. Fachliche Zusammenhänge

* **UC-01** berücksichtigt die Erkennung möglicher Dubletten, bevor ein neuer Kundendatensatz gespeichert wird.
* **UC-02** ermöglicht die Pflege bestehender Kundendaten.
* **UC-03** unterstützt den schnellen Zugriff auf vorhandene Kundeninformationen.
* **UC-04** stellt die nachvollziehbare Dokumentation von Kundenkontakten sicher.
* **UC-05** und **UC-06** unterstützen die Verwaltung und Fortschreibung von Vertriebschancen.
* **UC-07** ermöglicht der Vertriebsleitung, den Status relevanter Vertriebschancen zu überblicken.
* **UC-08** bildet die administrative Verwaltung von Benutzerberechtigungen ab.

## 6. Priorisierung für die weitere Modellierung

Für eine detaillierte Ausarbeitung werden zunächst folgende Use Cases ausgewählt:

1. **UC-01 – Kundendatensatz anlegen:** wichtig für Datenqualität und Dublettenvermeidung.
2. **UC-04 – Kundenkontakt dokumentieren:** wichtig für die Nachvollziehbarkeit von Kundenaktivitäten.
3. **UC-05 – Vertriebschance anlegen und verwalten:** wichtig für die Unterstützung des Vertriebsprozesses.

Diese Auswahl ist eine vorläufige Priorisierung für die Fallstudie. Sie ersetzt keine Abstimmung mit realen Stakeholdern.
