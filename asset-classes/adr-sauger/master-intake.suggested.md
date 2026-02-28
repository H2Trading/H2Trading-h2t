# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: ADR-Sauger

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (9 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `adr_zertifizierung` | 100% (9/9) |
| `arbeitsausstattung_zubehoer` | 100% (9/9) |
| `aufbau_tank_wasserrecycling` | 100% (9/9) |
| `elektrik_bordnetz` | 100% (9/9) |
| `fahrassistenzsysteme` | 100% (9/9) |
| `fahrerhaus_komfort` | 100% (9/9) |
| `hochdruckanlage` | 100% (9/9) |
| `steuerung_bedienung` | 100% (9/9) |
| `traegerfahrzeug` | 100% (9/9) |
| `sauganlage_vakuumsystem` | 89% (8/9) |
| `abmessungen` | 56% (5/9) |
| `abmessungen_gewichte` | 22% (2/9) |
| `dokumentation_konformitaet` | 11% (1/9) |
| `gewichte_betriebswerte` | 11% (1/9) |
| `gewichte_dimensionen` | 11% (1/9) |
| `sauganlage` | 11% (1/9) |
| `umwelt_emissionen` | 11% (1/9) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Aufbau Tank Wasserrecycling (`aufbau_tank_wasserrecycling`)

| Field path | Presence |
|---|---:|
| `aufbau_tank_wasserrecycling.hersteller` | 100% (9/9) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.hersteller` | 100% (9/9) |
| `traegerfahrzeug.modell` | 100% (9/9) |
| `traegerfahrzeug.achsen.konfiguration` | 89% (8/9) |

