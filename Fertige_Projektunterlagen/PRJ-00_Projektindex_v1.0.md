---
Projekt: H2 Trading GmbH
Dokument: PRJ-00 – Projektindex & Struktur
Version: v1.0
Status: gültig
Gültig ab: 2026-01-30
---

## Zweck

PRJ-00 definiert die **verbindliche Gesamtstruktur des Projekts H2 Trading GmbH**.

Dieses Dokument:
– ordnet alle PRJ-Regeln eindeutig ein  
– trennt PRJ-Regeln von operativen CASE-Threads  
– dient als stabiler Referenzpunkt für das gesamte Projekt  

PRJ-00 ist **Meta-Regelwerk** und wird nur bei strukturellen Änderungen angepasst.

---

## Projektstruktur – Überblick

Das Projekt besteht aus **PRJ-Regeln** und **operativen CASE-Threads**.

### 1. PRJ-Regeln (normativ, projektweit gültig)

PRJ-Dateien sind:
– dauerhaft gültig  
– versioniert (vMAJOR.MINOR)  
– als `.md` in den Projekteinstellungen abgelegt  
– Grundlage für alle CASE-Threads  

#### Verbindlicher PRJ-Satz

| PRJ | Titel |
|----|------|
| PRJ-00 | Projektindex & Struktur |
| PRJ-01 | Name & Marke |
| PRJ-02 | Firmenbuch & Rechtliches |
| PRJ-03 | Domain & Web |
| PRJ-04 | Marke & Corporate Design |
| PRJ-05 | Verträge & Dokumente (Meta) |
| PRJ-07 | Marketing & Online |
| PRJ-08 | Marktrecherche |
| PRJ-09 | Assettypen & Terminologie |
| PRJ-10 | Asset-Intake & Verkaufsprozess |
| PRJ-11 | Erlösmodell |
| PRJ-12 | Medienfactory & Bildverwendung |
| PRJ-13 | Datenverarbeitung | GPT |
| PRJ-14 | IT & Systeme |
| PRJ-15 | Dokumenten-Factory & Übersetzung |

**Nicht existent / bewusst ausgelassen:**
– PRJ-06 (Geschäftsmodell wird operativ als Kapitel geführt, nicht als PRJ)

---

## 2. Operative Arbeit – CASE-Threads

Operative Arbeit erfolgt **ausschließlich** in CASE-Threads.

### CASE-Thread-Logik

Ein CASE-Thread:
– behandelt **genau einen Case** (Transaktion / Projekt / Asset-Cluster)
– beginnt mit einem **Init-Prompt gemäß PRJ-00**
– nutzt PRJ-Regeln als verbindliche Grundlage
– erzeugt **konkrete Dokumente** (DOC-10-XX, DOC-05-XX)

**Namensschema:**

CASE H2T-YYYY-NNN – Kurzbeschreibung

Die CASE-Nummer wird **manuell vergeben** (keine automatische Zählung).

---

## 3. Dokumentenlogik (Kurzreferenz)

– Inhalte entstehen ausschließlich in Markdown  
– `_DE_FINAL.md` ist jeweilige inhaltliche Wahrheit  
– Word / PDF sind reine Ableitungen  
– Regeln hierzu: **PRJ-15**

Dokumenttypen:
– DOC-10-XX: Asset- & Verkaufsdokumente  
– DOC-05-XX: Vertrags- & Abwicklungsdokumente  

---

## 4. Archivierungsregel

– Abgeschlossene Threads werden **archiviert**
– Alte Kapitel-Threads werden **nicht weiterverwendet**
– Aktive Arbeit erfolgt immer:
  – entweder in einem PRJ-Thread (Regeländerung)
  – oder in einem CASE-Thread (operative Arbeit)

---

## 5. Änderungslogik

Änderungen an:
– PRJ-Dateien → neue PRJ-Version  
– Dokumentenregeln → PRJ-15  
– Projektstruktur → PRJ-00  

Keine impliziten oder stillen Änderungen.

---

## Status

Dieses Dokument bildet den **aktuellen, vollständigen Projektindex**  
und ist Grundlage für die weitere operative Arbeit.
