# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: TV-Kanalinspektionsfahrzeug

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
| `fahrerhaus_komfort` | 100% (1/1) |
| `hochdruckanlage` | 100% (1/1) |
| `sauganlage_vakuumsystem` | 100% (1/1) |
| `steuerung_bedienung` | 100% (1/1) |
| `traegerfahrzeug` | 100% (1/1) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Abmessungen Gewichte (`abmessungen_gewichte`)

| Field path | Presence |
|---|---:|
| `abmessungen_gewichte.gesamtgewicht_zulaessig_kg` | 100% (1/1) |
| `abmessungen_gewichte.radstand_mm` | 100% (1/1) |

### Arbeitsausstattung Zubehoer (`arbeitsausstattung_zubehoer`)

| Field path | Presence |
|---|---:|
| `arbeitsausstattung_zubehoer.hecktuer_oeffnungswinkel_grad` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.laderaumtrennwand` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.reserverad_typ` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.reserveradhalter_position` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.schiebetuer_rechts` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.verzurroesen_laderaum` | 100% (1/1) |
| `arbeitsausstattung_zubehoer.wagenheber` | 100% (1/1) |

### Elektrik Bordnetz (`elektrik_bordnetz`)

| Field path | Presence |
|---|---:|
| `elektrik_bordnetz.anzeige_waschwasserstand` | 100% (1/1) |
| `elektrik_bordnetz.aussenspiegel_blinkleuchte_integriert` | 100% (1/1) |
| `elektrik_bordnetz.aussenspiegel_elektrisch_verstellbar` | 100% (1/1) |
| `elektrik_bordnetz.aussenspiegel_heizbar` | 100% (1/1) |
| `elektrik_bordnetz.batterie_ah` | 100% (1/1) |
| `elektrik_bordnetz.bremsleuchte_dritte` | 100% (1/1) |
| `elektrik_bordnetz.leuchtweitenregelung` | 100% (1/1) |
| `elektrik_bordnetz.rundumkennleuchten_anzahl` | 100% (1/1) |
| `elektrik_bordnetz.verglasung_waermeschutz` | 100% (1/1) |

### Fahrerhaus Komfort (`fahrerhaus_komfort`)

| Field path | Presence |
|---|---:|
| `fahrerhaus_komfort.dachverkleidung` | 100% (1/1) |
| `fahrerhaus_komfort.handschuhfach_abschliessbar` | 100% (1/1) |
| `fahrerhaus_komfort.sitze_beifahrer` | 100% (1/1) |
| `fahrerhaus_komfort.sitze_fahrer` | 100% (1/1) |
| `fahrerhaus_komfort.zusatzheizung_luft_elektrisch` | 100% (1/1) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.antrieb.emission` | 100% (1/1) |
| `traegerfahrzeug.antrieb.kraftstofftank_l` | 100% (1/1) |
| `traegerfahrzeug.antrieb.motor_kw` | 100% (1/1) |
| `traegerfahrzeug.bremsen.bremsassistent` | 100% (1/1) |
| `traegerfahrzeug.fahrwerk.felgen_vorderachse` | 100% (1/1) |
| `traegerfahrzeug.federung.stabilisator_hinten` | 100% (1/1) |
| `traegerfahrzeug.federung.stabilisator_vorn_verstaerkt` | 100% (1/1) |
| `traegerfahrzeug.federung.stossdaempfer_verstaerkt` | 100% (1/1) |
| `traegerfahrzeug.hersteller` | 100% (1/1) |
| `traegerfahrzeug.modell` | 100% (1/1) |
| `traegerfahrzeug.sicherheit.airbag_fahrerseite` | 100% (1/1) |
| `traegerfahrzeug.sicherheit.kindersicherung` | 100% (1/1) |

