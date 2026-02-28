# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: ADR-Kombi

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (16 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `adr_zertifizierung` | 100% (16/16) |
| `arbeitsausstattung_zubehoer` | 100% (16/16) |
| `elektrik_bordnetz` | 100% (16/16) |
| `fahrassistenzsysteme` | 100% (16/16) |
| `fahrerhaus_komfort` | 100% (16/16) |
| `hochdruckanlage` | 100% (16/16) |
| `sauganlage_vakuumsystem` | 100% (16/16) |
| `steuerung_bedienung` | 100% (16/16) |
| `traegerfahrzeug` | 100% (16/16) |
| `aufbau_tank_wasserrecycling` | 88% (14/16) |
| `abmessungen` | 69% (11/16) |
| `abmessungen_gewichte` | 13% (2/16) |
| `aufbau_kanalreinigung` | 6% (1/16) |
| `aufbau_recycling_tank` | 6% (1/16) |
| `dokumente_wartung` | 6% (1/16) |
| `pto` | 6% (1/16) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Adr Zertifizierung (`adr_zertifizierung`)

| Field path | Presence |
|---|---:|
| `adr_zertifizierung.klassen` | 56% (9/16) |

### Arbeitsausstattung Zubehoer (`arbeitsausstattung_zubehoer`)

| Field path | Presence |
|---|---:|
| `arbeitsausstattung_zubehoer.leiter` | 44% (7/16) |
| `arbeitsausstattung_zubehoer.schraubstock` | 44% (7/16) |

### Hochdruckanlage (`hochdruckanlage`)

| Field path | Presence |
|---|---:|
| `hochdruckanlage.pumpe.druck_bar` | 50% (8/16) |
| `hochdruckanlage.pumpe.durchfluss_l_min` | 50% (8/16) |
| `hochdruckanlage.pumpe.modell` | 50% (8/16) |

### Sauganlage Vakuumsystem (`sauganlage_vakuumsystem`)

| Field path | Presence |
|---|---:|
| `sauganlage_vakuumsystem.pumpe.kapazitaet_m3_h` | 50% (8/16) |
| `sauganlage_vakuumsystem.pumpe.modell` | 50% (8/16) |
| `sauganlage_vakuumsystem.pumpe.vakuum_mbar` | 50% (8/16) |

### Steuerung Bedienung (`steuerung_bedienung`)

| Field path | Presence |
|---|---:|
| `steuerung_bedienung.fernbedienung.typ` | 50% (8/16) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.achsen.konfiguration` | 100% (16/16) |
| `traegerfahrzeug.hersteller` | 100% (16/16) |
| `traegerfahrzeug.modell` | 100% (16/16) |
| `traegerfahrzeug.antrieb.kraftstofftank_l` | 50% (8/16) |
| `traegerfahrzeug.antrieb.transmission` | 44% (7/16) |
| `traegerfahrzeug.pto.typ` | 44% (7/16) |

### Aufbau Tank Wasserrecycling (`aufbau_tank_wasserrecycling`)

| Field path | Presence |
|---|---:|
| `aufbau_tank_wasserrecycling.hersteller` | 88% (14/16) |
| `aufbau_tank_wasserrecycling.tank.typ_adr` | 63% (10/16) |
| `aufbau_tank_wasserrecycling.tank.entleerung` | 56% (9/16) |
| `aufbau_tank_wasserrecycling.tank.werkstoff` | 56% (9/16) |

