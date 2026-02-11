---
Projekt: H² Trading GmbH
Dokument: PRJ-00 – Master Projektregeln
Version: v1.3
Status: gültig
Gültig ab: 2026-01-30
---

## Zweck

PRJ-00 definiert die **projektweit verbindlichen Meta-Regeln**
für Struktur, Arbeitsweise, Thread-Logik, Dokumentenlogik
und Versionierung im Projekt H² Trading GmbH.

Dieses Dokument ist **normativ**.
Es beschreibt **wie gearbeitet wird**, nicht operative Inhalte.

---

## 1. Grundsatz: Dateien sind die Wahrheit

– Chats dienen ausschließlich der Erarbeitung, Diskussion und Korrektur  
– **Freigegebene Dateien** sind die einzige verbindliche Quelle  
– Ein freigegebenes Dokument ersetzt jede frühere Chatdiskussion  

➡️ Kein Dokument gilt als fertig, solange **keine Datei** freigegeben wurde.

---

## 2. Single Source of Truth (SSOT)

– Für jedes Dokument existiert **genau eine Master-Datei**  
– Master-Dateien liegen als `.md` vor  
– Ableitungen (Word, PDF, Übersetzungen) entstehen ausschließlich daraus  

➡️ Was nicht im Master-Markdown steht, **existiert nicht**.

---

## 3. Versionierungslogik (verbindlich)

– Versionierung ausschließlich nach Schema: `vMAJOR.MINOR`  
– **Keine Statusbegriffe im Dateinamen**  
  – kein „FINAL“
  – kein „CLEAN“
  – kein „FROZEN“
– Gültigkeit wird **nur im Header** definiert (`Status`, `Gültig ab`)  

➡️ Status ≠ Dateiname.

---

## 4. Thread-Logik

– Ein Thread = ein klar definierter Zweck  
– Zulässige Thread-Typen:
  – **PRJ-Threads** (Regeln / Meta)
  – **CASE-Threads** (konkrete operative Fälle)
– Keine Vermischung von Meta-Regeln und operativer Arbeit  

➡️ Zweckwechsel ⇒ neuer Thread.

---

## 5. CASE-Threads (operativ)

– Jeder operative Fall läuft in **genau einem CASE-Thread**  
– CASE-Threads enthalten:
  – Asset-Intake (DOC-10)
  – Anbieteranfrage
  – Exposé
  – Vertragsdokumente (DOC-05)
  – Übersetzungen & Builds
– Arbeiten erfolgen **end-to-end** pro Asset / Fall  

➡️ Keine Verteilung eines Assets über mehrere Threads.

---

## 6. STOP-Regel (verbindlich)

Arbeit wird **sofort gestoppt**, wenn:
– Projektregeln verletzt werden  
– Annahmen getroffen werden  
– Inhalte erfunden werden  
– Layout / Struktur abweicht  

➡️ Erst Klärung, dann Fortsetzung.

---

## 7. Freigabe-Logik

– Freigabe erfolgt **explizit** (z. B. „freigegeben“, „abgenommen“)  
– Nach Freigabe:
  – Dokument gilt als gültig
  – neue Version nur über neue `.md`
– Bei Freigabe wird:
  – die Datei vollständig ausgegeben
  – der **korrekte Dateiname** separat genannt  

➡️ Freigabe ist ein Zustand, kein Gefühl.

---

## 8. Verhältnis zu anderen PRJ

– PRJ-00 = **Meta-Rahmen**
– PRJ-10 = Inhalt & Prozesslogik (Asset / Verkauf)
– PRJ-12 = Medien & Bilder
– PRJ-15 = Dokumenten-Factory & Übersetzung  

➡️ Keine Dopplungen, klare Abgrenzung.

---

## Status

Dieses Dokument ist **gültig und verbindlich**  
Stand: 2026-01-30
