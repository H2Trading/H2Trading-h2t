Projekt: H2 Trading GmbH  
Dokument: PRJ-15 – Dokumenten-Factory & Übersetzung  
Version: v1.2  
Status: FREIGEGEBEN  
Letzte Freigabe: 2026-02-07  
Gültig ab: 2026-02-07  

---

## Zweck

PRJ-15 definiert die **projektweit verbindlichen Regeln**
zur Erstellung, Versionierung, Übersetzung und Ausgabe
aller Textdokumente im Projekt H2 Trading GmbH.

PRJ-15 ist die **normative Referenz** für alle Dokumenten-
Produktionsthreads (DOC-05-XX, DOC-10-XX usw.).

---

## Grundsatz – Single Source of Truth (SSOT)

– Markdown (`*.md`) ist die **einzige inhaltliche Wahrheit**  
– Word / PDF / Exposé sind **reine Ableitungen**  
– **Keine Bearbeitung in Word oder PDF zulässig**  
– Inhaltliche Änderungen erfolgen ausschließlich im Markdown  

Abweichungen gelten als **Fehler**, nicht als Stilfrage.

---

## Dokumenten- & Build-Logik

– Dokumente werden ausschließlich aus freigegebenen Markdown-Dateien erzeugt  
– Der Build ist **deterministisch und zustandslos**  
– Der Build erzeugt **keine eigenen Regeln oder Inhalte**  
– Fehlerhafte Builds gelten als **nicht erzeugt**

---

## Versionierung

– Versionierung verpflichtend nach Schema **vMAJOR.MINOR**  
– Status (ENTWURF / FREIGEGEBEN) steht **im Dokumentheader**, nicht im Dateinamen  
– Pro Sprache existiert **genau eine gültige freigegebene Version**  
– Neue Versionen entstehen ausschließlich durch neue Markdown-Dateien  

---

## Layout & Word-Vorlage

– Der Kaufvertrag ist die **verbindliche Layout-Referenz**  
– Einheitliche Typografie, Absätze und Einrückungen sind zwingend  
– Zulässige Word-Vorlage:
  – `PRJ-15_MASTER_WORD_LAYOUT_v1.0.docx`  
– Bei mehreren Versionen gilt **immer die höchste Versionsnummer**  
– Custom-Styles sind ausschließlich in der Master-Vorlage definiert  
– Der Build erzeugt **keine eigenen Styles**

---

## Markdown → Build (verbindliche Regeln)

– Keine leeren Word-Absätze  
– Manuelle Nummerierung, lokal pro §  
– Keine Word-Automatiknummerierung  
– Datenblöcke:
  – eine Markdown-Zeile = eine visuelle Zeile  
  – kein Einzug  
– Fortsetzungszeilen bleiben im selben Absatz  
– Inline-Markdown (`**fett**`) wird vollständig interpretiert  

---

## Übersetzung

– Übersetzungen sind **strikt 1:1**  
– Keine Kürzungen  
– Keine Ergänzungen  
– Keine inhaltlichen Anpassungen  
– Freigabe **je Sprache** zwingend  
– Übersetzungen erfolgen ausschließlich aus der freigegebenen DE-Version  

---

## Freigabe & Freeze

– Freigabe erfolgt explizit („freigegeben“, „abgenommen“)  
– Erst nach Freigabe dürfen Ableitungen erzeugt werden  
– Nach Freigabe:
  – keine stillschweigenden Änderungen  
  – neue Version nur über neue Markdown-Datei  

---

## Abgrenzung

PRJ-15 regelt **nicht**:
– Medien & Bilder → PRJ-12  
– Inhaltliche Assetlogik → PRJ-10  
– Terminologie & Assettypen → PRJ-09  
– Projektstruktur → PRJ-00  

---

## Geltungsbereich

Diese Regeln gelten:
– projektweit  
– threadübergreifend  
– für alle Dokumenttypen  
– für alle Sprachen  

---

**Status:** FREIGEGEBEN  
**Stand:** 2026-02-07
