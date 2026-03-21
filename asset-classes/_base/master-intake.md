# DOC-10-00 – Master Asset-Intake (BASE)

**Gültig für:** alle Assetklassen (Shared Base Template)  
**Version:** v0.1  
**Status:** MASTER (in Entwicklung)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** Pattern-Analyse `batch-pattern-analysis.md` (Universal Fields, 51 Assets)

> Dieses Base-Template definiert die universellen Sektionen des Asset-Intakes.
> Assetklassen-spezifische Master-Templates **erweitern** dieses Dokument um zusätzliche Module.

---

## Status (intern)

- **Asset-ID (intern, PRJ-09):** H2T-ASSET-YYYY-NNN
- **Assetklasse:** ___
- **Quelle / Inserat:** ___ (URL)
- **Externe ID / Anbieter-Referenz:** ___
- **Bearbeiter (H2T):** ___
- **Datum Intake:** ___

### Intake-Workflow / Freigaben
- **Datenstatus:**
  - ☐ Rohdaten (unverifiziert)
  - ☐ Teilverifiziert
  - ☐ Verifiziert (Exposé-fähig)
- **Bildfreigabe vorhanden:** ☐ Ja ☐ Nein ☐ Unklar

### Bewertung (intern)
- **Fit zum Portfolio:** ☐ Ja ☐ Nein ☐ Unklar
- **Priorität:** ☐ Hoch ☐ Mittel ☐ Niedrig
- **Risiko / Auffälligkeiten:** ___
- **Nächster Schritt:** ☐ Anbieter kontaktieren ☐ Besichtigung ☐ Unterlagen anfordern ☐ Sonstiges: ___

---

## Zweck dieses Dokuments

Dieses Dokument definiert den **verbindlichen Asset-Intake-Standard** der H2 Trading GmbH.
Es dient der strukturierten Erfassung von Assets, der internen Bewertung/Entscheidung
und ist die **Single Source of Truth (SSOT)** für abgeleitete Dokumente:

- DOC-10-00-A (Anbieterbestätigung / QA)
- DOC-10-01 (Exposé – nur verifizierte Daten, nur interne ID)

---

## A1 – Asset-Identifikation

- **Interne Asset-ID:** H2T-ASSET-YYYY-NNN
- **Asset-Typ / Assetklasse:** ___
- **Hersteller / Modell (Trägerfahrzeug):** ___
- **Achskonfiguration:** ___ (z. B. 6×2, 8×4)
- **Aufbau / System (Hersteller/Typ):** ___

---

## A2 – Eigentum & Verfügungsstatus

- **Anbieter:** ___ (Firma/Name)
- **Eigentumsstatus:**
  - ☐ Eigentum Anbieter
  - ☐ Leasing (noch laufend)
  - ☐ Finanzierung (noch laufend)
  - ☐ Sonstiges: ___
- **Verfügbarkeit:**
  - ☐ Sofort verfügbar
  - ☐ In Kürze verfügbar (voraussichtlich: ___)
  - ☐ Auf Anfrage
  - ☐ Reserviert
- **Standort:** ___

---

## A3 – Kurzbewertung Zustand

- **Zustand (Gesamteindruck):**
  - ☐ Neuwertig
  - ☐ Sehr gut
  - ☐ Gut
  - ☐ Gebrauchsspuren vorhanden
- **Kilometerstand (laut Anbieter):** ___
- **Erstzulassung:** ___
- **Baujahr:** ___
- **Letzte HU / §57a / TÜV:** ___
- **Bekannte Mängel / Abweichungen (Rohdaten):** ___

---

## A4 – Technische Daten (Universal-Module)

> Die folgenden Module wurden als **Universal Fields** in 7 Kategorien über 51 Assets identifiziert.
> (Quelle: Pattern-Analyse)

### A4.1 Trägerfahrzeug (`traegerfahrzeug`)

**Unterstruktur (BASE, min.):**
- Antrieb (Motor kW/PS, Abgasnorm, Getriebe, Kraftstoff)
- Achsen (Konfiguration, Achslasten, Eigenschaften)
- Bremsen
- Federung
- Fahrwerk (Rahmen, Rahmenüberhang, Kotflügel, Felgen/Reifen)
- Sicherheit (keine Redundanzen zu Assistenzsystemen)
- PTO / Nebenantrieb (falls vorhanden; ansonsten im Klassen-Template)

**Platzhalter:**
- Hersteller/Modell: ___
- Motor: ___
- Getriebe: ___
- Achsen: ___
- Fahrwerk: ___

### A4.2 Aufbau / Tank / Wasserrecycling (`aufbau_tank_wasserrecycling`)

**Platzhalter:**
- Hersteller Aufbau: ___
- Tanktyp / Material / Volumen: ___
- Entleerung / Besonderheiten: ___

### A4.3 Sauganlage / Vakuumsystem (`sauganlage_vakuumsystem`)

**Platzhalter:**
- Pumpe: ___
- Leistung / Vakuum: ___
- Saugschlauchsystem(e): ___ (DN, Länge, Position)

### A4.4 Hochdruckanlage (`hochdruckanlage`)

**Platzhalter:**
- Pumpe: ___
- Druck / Durchfluss: ___
- HD-Schlauchsystem(e): ___ (DN, Länge)

### A4.5 Steuerung / Bedienung (`steuerung_bedienung`)

**Platzhalter:**
- Bedienkonzept: ___
- Fernbedienung / CAN-BUS: ___

### A4.6 Fahrassistenzsysteme (`fahrassistenzsysteme`)

**Regel:** Nur Assistenzsysteme hier; Sicherheits-/Warnsysteme nicht doppelt unter Trägerfahrzeug.

**Platzhalter:**
- Rückfahrkamera: ☐ Ja ☐ Nein
- Verkehrszeichenerkennung: ☐ Ja ☐ Nein
- Fernlichtassistent: ☐ Ja ☐ Nein
- Sonstige: ___

### A4.7 Elektrik / Bordnetz (`elektrik_bordnetz`)

**Platzhalter:**
- Batterie: ___
- Steckdosen / Vorrüstung: ___
- Beleuchtung / LED: ___

### A4.8 ADR-Zertifizierung (`adr_zertifizierung`)

**Hinweis:** Bei nicht-ADR Klassen: Abschnitt kann leer bleiben.

**Platzhalter:**
- ADR Klassen/Typ: ___
- Prüfstatus / Hinweise: ___

### A4.9 Abmessungen & Gewichte (`abmessungen_gewichte`)

**Platzhalter:**
- zGG: ___ kg
- Leergewicht: ___ kg
- Nutzlast: ___ kg
- Abmessungen: ___

### A4.10 Arbeitsausstattung / Zubehör (`arbeitsausstattung_zubehoer`)

**Regel:** Minimal halten; alles was eindeutig in andere Module passt, dort einordnen.

**Platzhalter:**
- Werkzeugkasten / Halterungen / Leiter / etc.: ___

---

## A5 – Dokumente, Nachweise, Medien (universell)

- **Service-/Wartungsnachweise:** ☐ vorhanden ☐ teilweise ☐ nicht vorhanden
- **Technische Dokumentation (Aufbau/Aggregate):** ☐ vorhanden ☐ nicht vorhanden
- **Bilder vorhanden:** ☐ ja ☐ nein (Quelle/Ordner: ___)
- **Bildfreigabe (für Exposé):** ☐ ja ☐ nein ☐ offen

---

## Änderungslog

| Version | Datum | Änderung |
|---|---:|---|
| v0.1 | 2026-02-28 | Initial Base Template (Universal Fields + A1/A2/A3/Status/Bewertung) |
