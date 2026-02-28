# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: Vakuumsaugfass-Anhänger

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (5 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `adr_zertifizierung` | 100% (5/5) |
| `arbeitsausstattung_zubehoer` | 100% (5/5) |
| `aufbau_tank_wasserrecycling` | 100% (5/5) |
| `elektrik_bordnetz` | 100% (5/5) |
| `fahrassistenzsysteme` | 100% (5/5) |
| `fahrerhaus_komfort` | 100% (5/5) |
| `hochdruckanlage` | 100% (5/5) |
| `sauganlage_vakuumsystem` | 100% (5/5) |
| `steuerung_bedienung` | 100% (5/5) |
| `traegerfahrzeug` | 100% (5/5) |
| `abmessungen_gewichte` | 60% (3/5) |
| `abmessungen` | 40% (2/5) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Arbeitsausstattung Zubehoer (`arbeitsausstattung_zubehoer`)

| Field path | Presence |
|---|---:|
| `arbeitsausstattung_zubehoer.werkzeugkasten` | 60% (3/5) |
| `arbeitsausstattung_zubehoer.motorkiste_abschliessbar` | 40% (2/5) |
| `arbeitsausstattung_zubehoer.rungen_halterungen` | 40% (2/5) |

### Aufbau Tank Wasserrecycling (`aufbau_tank_wasserrecycling`)

| Field path | Presence |
|---|---:|
| `aufbau_tank_wasserrecycling.tank.werkstoff` | 80% (4/5) |
| `aufbau_tank_wasserrecycling.hersteller` | 40% (2/5) |
| `aufbau_tank_wasserrecycling.tank.entleerung` | 40% (2/5) |
| `aufbau_tank_wasserrecycling.tank.schmutzwasser_l` | 40% (2/5) |

### Sauganlage Vakuumsystem (`sauganlage_vakuumsystem`)

| Field path | Presence |
|---|---:|
| `sauganlage_vakuumsystem.pumpe.kapazitaet_m3_h` | 60% (3/5) |
| `sauganlage_vakuumsystem.pumpe.modell` | 60% (3/5) |
| `sauganlage_vakuumsystem.pumpe.vakuum_mbar` | 60% (3/5) |
| `sauganlage_vakuumsystem.sauglanze.dn` | 40% (2/5) |
| `sauganlage_vakuumsystem.sauglanze.laenge_m` | 40% (2/5) |
| `sauganlage_vakuumsystem.saugschlauch.dn` | 40% (2/5) |
| `sauganlage_vakuumsystem.saugschlauch.laenge_m` | 40% (2/5) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.fahrwerk.kotfluegel` | 80% (4/5) |
| `traegerfahrzeug.bremsen.typ` | 60% (3/5) |
| `traegerfahrzeug.fahrwerk.rahmen` | 60% (3/5) |
| `traegerfahrzeug.achsen.hinterachse.typ` | 40% (2/5) |

