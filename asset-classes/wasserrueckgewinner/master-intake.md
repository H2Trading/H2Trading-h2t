# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: Wasserrückgewinner

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (17 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `adr_zertifizierung` | 100% (17/17) |
| `arbeitsausstattung_zubehoer` | 100% (17/17) |
| `elektrik_bordnetz` | 100% (17/17) |
| `hochdruckanlage` | 100% (17/17) |
| `steuerung_bedienung` | 100% (17/17) |
| `traegerfahrzeug` | 100% (17/17) |
| `fahrerhaus_komfort` | 94% (16/17) |
| `sauganlage_vakuumsystem` | 94% (16/17) |
| `aufbau_tank_wasserrecycling` | 88% (15/17) |
| `fahrassistenzsysteme` | 82% (14/17) |
| `abmessungen` | 53% (9/17) |
| `abmessungen_gewichte` | 24% (4/17) |
| `assistenzsysteme` | 18% (3/17) |
| `aufbau_tank` | 12% (2/17) |
| `allgemeine_daten` | 6% (1/17) |
| `dokument_metadaten` | 6% (1/17) |
| `kabine_komfort` | 6% (1/17) |
| `sauganlage` | 6% (1/17) |
| `sicherheitsausstattung` | 6% (1/17) |
| `sonderoptionen` | 6% (1/17) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.hersteller` | 100% (17/17) |
| `traegerfahrzeug.modell` | 100% (17/17) |
| `traegerfahrzeug.achsen.konfiguration` | 94% (16/17) |

### Aufbau Tank Wasserrecycling (`aufbau_tank_wasserrecycling`)

| Field path | Presence |
|---|---:|
| `aufbau_tank_wasserrecycling.hersteller` | 88% (15/17) |

