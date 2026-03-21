# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: Elektro-Fahrgestell

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (1 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `abmessungen_gewichte` | 100% (1/1) |
| `adr_zertifizierung` | 100% (1/1) |
| `arbeitsausstattung_zubehoer` | 100% (1/1) |
| `aufbau_tank_wasserrecycling` | 100% (1/1) |
| `elektrik_bordnetz` | 100% (1/1) |
| `fahrassistenzsysteme` | 100% (1/1) |
| `hochdruckanlage` | 100% (1/1) |
| `sauganlage_vakuumsystem` | 100% (1/1) |
| `sonderoptionen` | 100% (1/1) |
| `steuerung_bedienung` | 100% (1/1) |
| `traegerfahrzeug` | 100% (1/1) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Abmessungen Gewichte (`abmessungen_gewichte`)

| Field path | Presence |
|---|---:|
| `abmessungen_gewichte.zulaessiges_gesamtgewicht_kg` | 100% (1/1) |

### Elektrik Bordnetz (`elektrik_bordnetz`)

| Field path | Presence |
|---|---:|
| `elektrik_bordnetz.batterie_spannung_v` | 100% (1/1) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.achskonfiguration.typ` | 100% (1/1) |
| `traegerfahrzeug.antrieb.energiequelle` | 100% (1/1) |
| `traegerfahrzeug.antrieb.leistung_kw` | 100% (1/1) |
| `traegerfahrzeug.antrieb.leistung_ps` | 100% (1/1) |
| `traegerfahrzeug.antrieb.max_drehmoment_nm` | 100% (1/1) |
| `traegerfahrzeug.antrieb.motortyp` | 100% (1/1) |
| `traegerfahrzeug.antrieb.nennspannung_v` | 100% (1/1) |
| `traegerfahrzeug.antrieb.spitzenleistung_kw` | 100% (1/1) |
| `traegerfahrzeug.fahrwerk.bereifung_hinterachse` | 100% (1/1) |
| `traegerfahrzeug.fahrwerk.bereifung_vorderachse` | 100% (1/1) |
| `traegerfahrzeug.federung.hinterachse` | 100% (1/1) |
| `traegerfahrzeug.federung.vorderachse` | 100% (1/1) |
| `traegerfahrzeug.hersteller` | 100% (1/1) |
| `traegerfahrzeug.modell` | 100% (1/1) |

