# DOC-10-00 – Master Asset-Intake (SUGGESTED)
Assetklasse: Kanalreinigungsfahrzeug

**Status:** SUGGESTED (aus Datenpool abgeleitet)  
**Letzte Änderung:** 2026-02-28  
**Quelle:** asset-data-final.json pool (2 Assets), Template-Threshold 40%

**Base:** ../_base/master-intake.md

---

## Hinweis

Dieses Dokument ist ein automatisch abgeleiteter Vorschlag.
Bitte fachlich reviewen und anschließend in `master-intake.md` übernehmen (oder Teile daraus).

---

## Modules (Top-Level Keys)

| Modul | Presence |
|---|---:|
| `adr_zertifizierung` | 100% (2/2) |
| `arbeitsausstattung_zubehoer` | 100% (2/2) |
| `aufbau_tank_wasserrecycling` | 100% (2/2) |
| `elektrik_bordnetz` | 100% (2/2) |
| `fahrassistenzsysteme` | 100% (2/2) |
| `fahrerhaus_komfort` | 100% (2/2) |
| `hochdruckanlage` | 100% (2/2) |
| `sauganlage_vakuumsystem` | 100% (2/2) |
| `steuerung_bedienung` | 100% (2/2) |
| `traegerfahrzeug` | 100% (2/2) |
| `abmessungen` | 50% (1/2) |
| `abmessungen_gewichte` | 50% (1/2) |

---

## Feldkandidaten je Modul (>= 40% Presence)

### Adr Zertifizierung (`adr_zertifizierung`)

| Field path | Presence |
|---|---:|
| `adr_zertifizierung.geschwindigkeitsbegrenzer` | 50% (1/2) |

### Arbeitsausstattung Zubehoer (`arbeitsausstattung_zubehoer`)

| Field path | Presence |
|---|---:|
| `arbeitsausstattung_zubehoer.anhaengerkupplung` | 50% (1/2) |
| `arbeitsausstattung_zubehoer.einstiegsgriff` | 50% (1/2) |
| `arbeitsausstattung_zubehoer.markierungsleuchten` | 50% (1/2) |
| `arbeitsausstattung_zubehoer.schmutzfaenger_hinten` | 50% (1/2) |
| `arbeitsausstattung_zubehoer.zuziehhilfe_schiebetuer` | 50% (1/2) |

### Aufbau Tank Wasserrecycling (`aufbau_tank_wasserrecycling`)

| Field path | Presence |
|---|---:|
| `aufbau_tank_wasserrecycling.hersteller` | 100% (2/2) |

### Elektrik Bordnetz (`elektrik_bordnetz`)

| Field path | Presence |
|---|---:|
| `elektrik_bordnetz.batterie_ah` | 50% (1/2) |
| `elektrik_bordnetz.batterietrennschalter` | 50% (1/2) |
| `elektrik_bordnetz.generator_a` | 50% (1/2) |
| `elektrik_bordnetz.steckdosen` | 50% (1/2) |
| `elektrik_bordnetz.zusatzbatterie` | 50% (1/2) |

### Fahrassistenzsysteme (`fahrassistenzsysteme`)

| Field path | Presence |
|---|---:|
| `fahrassistenzsysteme.abbiege_assistent` | 50% (1/2) |
| `fahrassistenzsysteme.aktiver_bremsassistent` | 50% (1/2) |
| `fahrassistenzsysteme.aktiver_spurhalteassistent` | 50% (1/2) |
| `fahrassistenzsysteme.anfahrinformations_assistent` | 50% (1/2) |
| `fahrassistenzsysteme.attention_assist` | 50% (1/2) |
| `fahrassistenzsysteme.intelligenter_geschwindigkeits_assistent` | 50% (1/2) |
| `fahrassistenzsysteme.pannenmanagement` | 50% (1/2) |
| `fahrassistenzsysteme.rueckfahrkamera` | 50% (1/2) |
| `fahrassistenzsysteme.seitenwind_assistent` | 50% (1/2) |
| `fahrassistenzsysteme.verkehrszeichenerkennung` | 50% (1/2) |

### Fahrerhaus Komfort (`fahrerhaus_komfort`)

| Field path | Presence |
|---|---:|
| `fahrerhaus_komfort.klimaanlage` | 50% (1/2) |
| `fahrerhaus_komfort.multimedia_cockpit` | 50% (1/2) |
| `fahrerhaus_komfort.navigationssystem` | 50% (1/2) |
| `fahrerhaus_komfort.scheibenwischer` | 50% (1/2) |
| `fahrerhaus_komfort.sitze` | 50% (1/2) |

### Steuerung Bedienung (`steuerung_bedienung`)

| Field path | Presence |
|---|---:|
| `steuerung_bedienung.fernbedienung.typ` | 50% (1/2) |

### Traegerfahrzeug (`traegerfahrzeug`)

| Field path | Presence |
|---|---:|
| `traegerfahrzeug.hersteller` | 100% (2/2) |
| `traegerfahrzeug.modell` | 100% (2/2) |
| `traegerfahrzeug.achsen.konfiguration` | 50% (1/2) |
| `traegerfahrzeug.achsen.vorderachse.eigenschaften` | 50% (1/2) |
| `traegerfahrzeug.antrieb.emission` | 50% (1/2) |
| `traegerfahrzeug.antrieb.kraftstofftank_l` | 50% (1/2) |
| `traegerfahrzeug.antrieb.motor_kw` | 50% (1/2) |
| `traegerfahrzeug.bremsen.adaptives_bremslicht` | 50% (1/2) |
| `traegerfahrzeug.bremsen.anfahrhilfe` | 50% (1/2) |
| `traegerfahrzeug.fahrwerk.radstand_mm` | 50% (1/2) |
| `traegerfahrzeug.fahrwerk.rahmen` | 50% (1/2) |
| `traegerfahrzeug.federung.stabilisierung` | 50% (1/2) |
| `traegerfahrzeug.pto.getriebesperre` | 50% (1/2) |
| `traegerfahrzeug.pto.typ` | 50% (1/2) |
| `traegerfahrzeug.sicherheit.airbags.beifahrer` | 50% (1/2) |
| `traegerfahrzeug.sicherheit.airbags.fahrer` | 50% (1/2) |
| `traegerfahrzeug.sicherheit.reifendruck_kontrolle` | 50% (1/2) |
| `traegerfahrzeug.sicherheit.sicherheitsgurt_warnung` | 50% (1/2) |
| `traegerfahrzeug.sicherheit.totwinkel_assistent` | 50% (1/2) |

### Abmessungen (`abmessungen`)

| Field path | Presence |
|---|---:|
| `abmessungen.zgg_kg` | 50% (1/2) |

