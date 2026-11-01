# UC-01 – Kundendatensatz anlegen

## 1. Allgemeine Informationen

| Attribut                 | Beschreibung                                       |
| ------------------------ | -------------------------------------------------- |
| Use-Case-ID              | UC-01                                              |
| Name                     | Kundendatensatz anlegen                            |
| Primärer Akteur          | Vertriebsmitarbeitende                             |
| Beteiligtes System       | CRM-System                                         |
| Zugehörige Anforderungen | BR-01, BR-03, FR-01, FR-03, NFR-02, NFR-03, NFR-05 |
| Priorität                | Hoch                                               |

## 2. Ziel

Der Use Case beschreibt, wie berechtigte Vertriebsmitarbeitende einen neuen Kundendatensatz im CRM-System anlegen und dabei mögliche Dubletten erkennen können.

## 3. Vorbedingungen

* Der Benutzer ist im CRM-System angemeldet.
* Der Benutzer verfügt über die Berechtigung, Kundendatensätze anzulegen.
* Das CRM-System ist verfügbar.

## 4. Auslöser

Der Benutzer möchte einen neuen Kunden im CRM-System erfassen.

## 5. Hauptablauf

1. Der Benutzer öffnet die Funktion zum Anlegen eines neuen Kundendatensatzes.
2. Das System zeigt die Eingabemaske für Kundendaten an.
3. Der Benutzer gibt die erforderlichen Kundeninformationen ein.
4. Der Benutzer startet die Prüfung und Speicherung des Datensatzes.
5. Das System prüft, ob alle Pflichtfelder ausgefüllt sind.
6. Das System prüft anhand definierter Identifikationsmerkmale, ob mögliche Dubletten existieren.
7. Das System zeigt an, dass keine mögliche Dublette erkannt wurde.
8. Das System speichert den neuen Kundendatensatz.
9. Das System bestätigt die erfolgreiche Speicherung und zeigt den angelegten Datensatz an.

## 6. Alternative und Ausnahmeabläufe

### A1 – Pflichtfelder fehlen

1. Das System stellt fest, dass mindestens ein Pflichtfeld nicht ausgefüllt wurde.
2. Das System zeigt einen verständlichen Hinweis auf die fehlenden Angaben an.
3. Der Benutzer ergänzt die erforderlichen Informationen.
4. Der Ablauf wird mit Schritt 4 des Hauptablaufs fortgesetzt.

**Ergebnis:** Der Datensatz wird erst gespeichert, wenn die erforderlichen Pflichtangaben vollständig sind.

### A2 – Mögliche Dublette erkannt

1. Das System erkennt anhand definierter Identifikationsmerkmale einen möglichen bestehenden Kundendatensatz.
2. Das System zeigt die relevanten Vergleichsinformationen an.
3. Der Benutzer prüft den bestehenden Datensatz.

Anschließend bestehen folgende Möglichkeiten:

* **A2.1 – Bestehender Kunde gefunden:** Der Benutzer bricht die Neuanlage ab und verwendet den bestehenden Datensatz.
* **A2.2 – Keine tatsächliche Dublette:** Der Benutzer bestätigt, dass die Neuanlage fortgesetzt werden soll, sofern dies nach den fachlich festgelegten Regeln zulässig ist.

**Offene Klärung:** Die Regeln für den Umgang mit möglichen Dubletten und die Berechtigung zur Fortsetzung müssen fachlich abgestimmt werden.

### A3 – Benutzer ist nicht berechtigt

1. Das System stellt fest, dass der Benutzer keine Berechtigung zur Neuanlage besitzt.
2. Das System verweigert den Zugriff auf die Funktion beziehungsweise verhindert das Speichern.
3. Das System informiert den Benutzer über die fehlende Berechtigung.

**Ergebnis:** Es wird kein neuer Kundendatensatz angelegt.

### A4 – Speichern schlägt fehl

1. Das System kann den Datensatz aufgrund eines technischen Fehlers nicht speichern.
2. Das System informiert den Benutzer über den fehlgeschlagenen Speichervorgang.
3. Das System zeigt an, dass der Datensatz nicht erfolgreich angelegt wurde.

**Ergebnis:** Der Benutzer kann den Vorgang erneut versuchen, sobald die Ursache behoben ist.

## 7. Nachbedingungen

### Erfolgsfall

* Der neue Kundendatensatz ist im CRM-System gespeichert.
* Der Datensatz besitzt eine eindeutige Identifikation.
* Der Benutzer erhält eine Bestätigung über die erfolgreiche Anlage.

### Fehler- oder Abbruchfall

* Es wurde kein neuer Kundendatensatz angelegt.
* Bereits vorhandene Kundendaten wurden durch den abgebrochenen Vorgang nicht verändert.

## 8. Geschäftsregeln

| ID       | Geschäftsregel                                                                                                   |
| -------- | ---------------------------------------------------------------------------------------------------------------- |
| BRULE-01 | Alle fachlich definierten Pflichtfelder müssen vor der Speicherung ausgefüllt sein.                              |
| BRULE-02 | Vor der Neuanlage muss eine Prüfung auf mögliche Dubletten anhand festgelegter Identifikationsmerkmale erfolgen. |
| BRULE-03 | Kundendatensätze dürfen nur durch entsprechend berechtigte Benutzer angelegt werden.                             |
| BRULE-04 | Ein möglicher Dublettentreffer darf nicht automatisch als bestätigte Dublette behandelt werden.                  |

## 9. Offene Fragen

* Welche Kundeninformationen sind Pflichtfelder?
* Welche Identifikationsmerkmale werden für die Dublettenprüfung verwendet?
* Darf eine Neuanlage trotz eines möglichen Dublettentreffers fortgesetzt werden?
* Welche Informationen dürfen Benutzer bei fehlender Berechtigung sehen?
* Wie soll das System mit einem fehlgeschlagenen Speichervorgang umgehen?

## 10. Abnahmekriterien

Der Use Case gilt fachlich als erfüllt, wenn:

* berechtigte Benutzer Kundendatensätze anlegen können,
* fehlende Pflichtfelder erkannt und gemeldet werden,
* mögliche Dubletten anhand definierter Regeln erkannt werden,
* unberechtigte Neuanlagen verhindert werden,
* erfolgreiche und fehlgeschlagene Speichervorgänge eindeutig erkennbar sind.
