Projekt: H² Trading GmbH  
Dokument: PRJ-13 – Datenverarbeitung & GPT  
Version: v1.0  
Status: FREIGEGEBEN  
Letzte Freigabe: 2026-02-07  
Gültig ab: 2026-02-07  

---

## Zweck

PRJ-13 definiert die **projektweit verbindlichen Grundsätze**
für den Einsatz von GPT und vergleichbaren Systemen
zur Datenverarbeitung im Projekt H² Trading GmbH.

PRJ-13 ist **normativ und systemlogisch**, nicht operativ.  
Es regelt **was GPT darf und was nicht**, keine Implementierungen.

---

## Verbindlicher Hinweis

❗ Keine Tool-Auswahl oder Systemarchitektur  
❗ Keine Automatisierungs- oder Workflow-Implementierung  
❗ Keine operativen Prompt-Designs  
❗ Keine Entscheidungsdelegation an GPT  

---

## Fixe Entscheidungen (Meta)

– GPT dient als:
  – Analysehilfe  
  – Strukturierungswerkzeug  
  – Text- und Datenverarbeitungssystem  

– Verarbeitung **ausschließlich explizit bereitgestellter Daten**  
– Keine eigenständige Datenerhebung durch GPT  
– Ergebnisse sind:
  – interne Arbeitsgrundlage  
  – **keine** Entscheidungsfinalisierung  

---

## Datenquellen & Grenzen

Zulässig:
– vom Nutzer bereitgestellte Texte, Tabellen, Dokumente  
– explizit bereitgestellte Assetdaten (DOC-10-00)  
– explizit übergebene Bilder (nur dann)

Unzulässig:
– implizite Annahmen  
– Rekonstruktionen aus Kontext  
– Auffüllen fehlender Daten  
– eigenständige Recherche ohne Auftrag & Quellenpflicht  

---

## Reproduzierbarkeit

– Aussagen müssen aus Daten ableitbar sein  
– Interpretationen sind explizit zu kennzeichnen  
– Keine scheinbar faktischen Aussagen ohne Grundlage  
– Recherche ≠ Bewertung (strikte Trennung)

---

## Umgang mit sensiblen Daten

– Verarbeitung nur bei expliziter Bereitstellung  
– Nach Möglichkeit anonymisiert / abstrahiert  
– Keine Speicherung über den Kontext hinaus  

---

## Abgrenzung zu PRJ-12 (Medien)

– Bilder sind **keine SSOT**  
– Keine Annahmen über Bildinhalte  
– Bildstatus nur:
  – vorliegend / nicht vorliegend / unbekannt  

---

## Abgrenzung zu PRJ-15 (Dokumente)

– Keine Layout-, Build- oder Übersetzungslogik  
– Keine Dokumentenproduktion  
– Keine Versionierungsregeln  

---

## Wirkt auf

– PRJ-00 – Projektindex  
– PRJ-08 – Marktrecherche  
– PRJ-09 – Assettypen & Terminologie  
– PRJ-10 – Asset-Intake  
– PRJ-12 – Medienfactory  
– PRJ-15 – Dokumentenfactory  
– DOC-10-XX / DOC-05-XX  

---

## No-Gos

– Keine stillen Annahmen  
– Kein GPT als Black-Box-Entscheider  
– Keine operativen Automationen  

---

**Status:** FREIGEGEBEN  
**Stand:** 2026-02-07
