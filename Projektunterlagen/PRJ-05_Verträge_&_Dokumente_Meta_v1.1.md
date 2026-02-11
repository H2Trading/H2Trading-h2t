---
Projekt: H² Trading GmbH
Dokument: PRJ-05 – Verträge & Dokumente (Meta)
Version: v1.1
Status: gültig
Gültig ab: 2026-02-07
---

## Zweck

PRJ-05 definiert die **projektweit verbindliche Meta-Logik**
für alle Vertrags-, Abwicklungs- und dokumentennahen Inhalte.

Dieses Dokument regelt **nicht** die Erstellung einzelner Verträge,
sondern die **Struktur, Abgrenzung und Geltung** aller Dokumenttypen
(DOC-05-XX, DOC-10-XX).

PRJ-05 ist **normativ**, nicht operativ.

---

## Grundsatz: Dokumente sind die Wahrheit

– Freigegebene Dokumente sind verbindlich  
– Chats dienen ausschließlich der Erarbeitung  
– Ein freigegebenes Dokument ersetzt jede frühere Diskussion  
– Es existiert **keine implizite Verbindlichkeit**  

Kein Dokument gilt als abgeschlossen,
solange keine Datei freigegeben ist.

---

## Dokumenttypen & Nummernkreise

### DOC-05-XX – Vertrags- & Abwicklungsdokumente

Umfasst u. a.:

– DOC-01 Kaufvertrag (B2B)
– DOC-02 Übergabeprotokoll
– DOC-03 Vermittlungsvertrag
– DOC-04 Vollmacht / Exportvollmacht
– DOC-05 AGB des Vermittlers
– DOC-06 Rechnung / Provisionsabrechnung
– DOC-07 Unterlagenliste
– DOC-08 Auftragsannahme Zusatzleistungen

Grundsatz:
– DOC-05-XX regeln **Rechtsverhältnisse**
– DOC-05-XX sind **keine Marketing- oder Verkaufsdokumente**

---

### DOC-10-XX – Assetbezogene Dokumente

– DOC-10-00 Asset-Intake (intern, SSOT)
– DOC-10-00-A Asset-Intake (Anbieterfassung)
– DOC-10-01 Asset-Exposé (extern, nicht vertraglich)

DOC-10-XX:
– enthalten **keine Vertragslogik**
– enthalten **keine Preis- oder Provisionsregelungen**

---

## Zentrale Abgrenzungen (verbindlich)

### Kaufvertrag

– Vertragsparteien: Verkäufer ↔ Käufer  
– Vermittler ist **nie Vertragspartei**  
– Gewährleistungsausschluss / „gekauft wie gesehen“  
– Gerichtsstand gemäß Kapitel „Rechtliches“ (PRJ-02)

---

### Vermittlungsvertrag

– Vertragsparteien: Vermittler ↔ Verkäufer  
– Keine Erfolgsgarantie  
– Klare Haftungsabgrenzung  
– Vergütung ausschließlich gemäß Vertrag  
– Gerichtsstand: Wien, Österreich

---

### Zusatzleistungen

– Immer **separat** zu beauftragen  
– Eigener Dokumenttyp (DOC-08)  
– Keine implizite Haftungserweiterung  
– Keine stillschweigende Leistungspflicht

---

## Single Source of Truth (SSOT)

– Markdown (`*_DE_FINAL.md`) ist **einzige inhaltliche Wahrheit**
– Word / PDF sind **reine Ableitungen**
– Keine Bearbeitung in Word oder PDF zulässig
– Änderungen nur:
  – versioniert
  – explizit
  – nachvollziehbar

---

## Layout & Dokumenten-Factory

– Einheitliches Masterlayout verpflichtend  
– Referenz: Kaufvertrag  
– Build-Regeln gemäß PRJ-15  
– Keine dokumentenspezifischen Sonderlayouts  

Abweichungen gelten als **Fehler**, nicht als Stilfrage.

---

## Übersetzung & Versionierung

– Übersetzungen strikt 1:1  
– Keine Kürzungen  
– Keine Ergänzungen  
– Keine inhaltlichen Anpassungen  

Versionierung:
– vMAJOR.MINOR
– keine Statusbegriffe („FINAL“) im Dateinamen
– Status ausschließlich im Dokumentkopf

---

## STOP-Regel (verbindlich)

Bei Unklarheiten gilt:

**STOPP – keine Weiterarbeit**

Auslöser u. a.:
– Regelkonflikt PRJ-05 ↔ PRJ-15
– Unklare Dokumentenzuordnung
– Abweichung vom Masterlayout
– Versuch einer Bearbeitung außerhalb des SSOT

---

## Wirkt auf folgende Projektbereiche

– PRJ-02 Firmenbuch & Rechtliches
– PRJ-06 Geschäftsmodell
– PRJ-10 Asset-Intake & Verkaufsprozess
– PRJ-15 Dokumenten-Factory & Übersetzung
– alle DOC-05-XX
– alle DOC-10-XX

---

## Status

Dieses Dokument ist **gültig**  
Änderungen nur über neue Version.
