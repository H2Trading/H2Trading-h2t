---
Projekt: H² Trading GmbH
Dokument: PRJ-14 – IT & Systeme
Version: v1.0
Status: FINAL
Letzte Freigabe: 2026-01-29
Gültig ab: 2026-01-29
---

## Zweck

PRJ-14 definiert die **projektweit verbindlichen Leitplanken**
für IT, Datenhaltung und Systemgrenzen.

Das Dokument ist **normativ** und legt Prinzipien fest,
keine konkreten Systeme, Tools oder Implementierungen.

---

## Grundsatz

IT-Systeme dienen der **Umsetzung projektlogischer Regeln**,
nicht deren Definition.

Fachliche Wahrheit, Struktur und Ordnung
werden ausschließlich in den jeweiligen PRJ- und DOC-Dokumenten festgelegt.

---

## Verbindliche Leitplanken

### 1. Systemtrennung

Projektweit gilt eine strikte Trennung von:

– Datenhaltung  
– Prozesslogik  
– Ausgabekanälen  

Vermischungen (z. B. Logik im Frontend, Wahrheit im Dokument)
sind unzulässig.

---

### 2. Single Source of Truth (SSOT)

– Inhaltliche Wahrheiten entstehen **nicht** in IT-Systemen  
– IT-Systeme replizieren, speichern oder transportieren Daten  
– Die fachliche SSOT liegt außerhalb der Systeme  
– Redundante Wahrheiten sind unzulässig  

---

### 3. Dokumente & Inhalte

– Textdokumente entstehen ausschließlich über die Dokumenten-Factory  
– Es existiert **keine** manuelle Dokumentenerstellung  
– Systeme erzeugen keine eigenen Dokumentinhalte  
– Inhalte werden nicht systemintern verändert  

Referenz: PRJ-15 – Dokumenten-Factory & Übersetzung

---

### 4. Medien & Bilder

– Bilder sind keine inhaltliche Wahrheit  
– Systeme speichern Medien getrennt von Textlogik  
– Medienfreigaben erfolgen nicht automatisch  
– IT-Systeme setzen ausschließlich Freigabestatus um  

Referenz: PRJ-12 – Medienfactory & Bildverwendung

---

### 5. Datenpflege & Redundanz

– Keine doppelte Datenpflege  
– Keine parallelen Datensätze mit eigener Wahrheit  
– Systeme dürfen Daten spiegeln, nicht interpretieren  
– Synchronisation ersetzt keine inhaltliche Klärung  

---

### 6. Systemoffenheit

– PRJ-14 trifft **keine** Aussagen zu:
  – ERP
  – DMS
  – PIM
  – CRM
  – Workflow-Engines

– Systeme sind austauschbar  
– Projektlogik bleibt unabhängig von Tool-Entscheidungen  

---

### 7. Abgrenzung zu anderen PRJ

PRJ-14 regelt **nicht**:

– Asset-Inhalte oder Prozesse (→ PRJ-10)  
– Dokumentenerstellung oder Übersetzung (→ PRJ-15)  
– Bildbearbeitung oder Medienlogik (→ PRJ-12)  
– Vertragslogik oder Inhalte (→ Kapitel 05 / DOC-05-XX)  

---

## Status

FINAL – verbindlich eingefroren
