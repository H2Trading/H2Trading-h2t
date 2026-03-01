# ROADMAP-01: Provider-Portal + Admin Dashboard

**Status:** 💡 Planned (not started)  
**Priority:** Medium (after batch-regeneration complete)  
**Estimated Effort:** 48h (MVP: 10h)  
**Created:** 2026-03-01  
**Author:** Captain Kirk (OpenClaw)

---

## Vision

**Automatisierter Provider Self-Service für Asset-Verifizierung:**
- Provider erhalten Link zu ihrer Anbieteranfrage (DOC-10-00-A)
- Können fehlende Pflichtfelder direkt ausfüllen
- Bestätigen vorhandene Daten per Checkbox
- Digital signieren (Name + Timestamp)
- System sendet Auto-Bestätigung per Mail

**Internes Admin Dashboard:**
- Asset-Klassen verwalten (CRUD)
- Pflichtfelder-Taxonomie (HARD/SOFT) per UI editieren
- Master-Templates bearbeiten (Markdown → Preview)
- Batch-Actions triggern ("Regenerate all 51 assets")

---

## Business Value

### 1. Skalierbarkeit
**Problem:** 51+ Assets manuell zu verifizieren = nicht tragbar  
**Lösung:** Self-Service → 0h manuelle Arbeit pro Asset

### 2. Professionalität
**Problem:** E-Mail Ping-Pong wirkt unprofessionell  
**Lösung:** Branded Portal mit klarem Workflow

### 3. Datenqualität
**Problem:** Copy-Paste-Fehler bei manueller Übertragung  
**Lösung:** Provider korrigiert direkt im System

### 4. Compliance
**Problem:** Kein Audit-Trail (wer hat wann was bestätigt)  
**Lösung:** Timestamp + Provider-Name gespeichert

---

## ROI Kalkulation

**Manueller Prozess:**
- 51 Assets × 15 Min/Asset = **12.75h** (E-Mail hin/her, Copy-Paste, Nachfragen)
- Bei 100 Assets/Monat = **25h/Monat** manuelle Arbeit

**Automatisierter Prozess:**
- **Einmalig:** 10h Entwicklung (MVP)
- **Laufend:** 0h pro Asset (nur Monitoring)

**Break-Even:** Nach 1 Batch (51 Assets)  
**ROI bei 100 Assets/Monat:** 25h gespart × 12 Monate = **300h/Jahr**

---

## Components

### Component 1: Provider-Portal

**Features (MVP):**
- ✅ Token-basierter Login (unique Link pro Asset)
- ✅ DOC-10-00-A Anzeige (read-only)
- ✅ Checkboxen für Bestätigungen (A3a, A4b, A5)
- ✅ Digital Stamp (Provider-Name + Timestamp)
- ✅ Auto-Mail (Bestätigung an H2T + Provider)

**Features (Full):**
- ✅ Fehlende Pflichtfelder als Formular (zGG, Motorleistung, etc.)
- ✅ Validation + Error Messages
- ✅ Diff-Report (was wurde geändert)
- ✅ File-Upload für Dokumente (COC, Service-Historie)

**Tech Stack:**
- Backend: Node.js (Express)
- Frontend: Server-rendered HTML (kein React nötig)
- Auth: Token-based (kein Passwort, Link = Secret)
- Storage: JSON files + GitHub commit (SSOT)
- Mail: Brevo API (bereits integriert)

**Effort:**
- MVP (read-only + confirm): **10h**
- Full (edit + upload): **18h**

---

### Component 2: Admin Dashboard

**Features:**
- ✅ Asset-Klassen Verwaltung (CRUD)
- ✅ Pflichtfelder-Editor (HARD/SOFT Klassifikation per UI)
- ✅ Master-Template-Editor (Markdown mit Live-Preview)
- ✅ Batch-Actions ("Regenerate all 51 assets" Button)
- ✅ Statistics (51 Assets, 10 Klassen, Completion %)

**Tech Stack:**
- Backend: Node.js API
- Frontend: Minimal (könnte auch statisches HTML sein)
- Storage: GitHub (SSOT bleibt, UI ist nur Editor)
- Auth: Basic Auth (wie aktuelles Dashboard)

**Effort:**
- Admin Dashboard: **20h**

---

### Component 3: Integration

**Workflow:**
1. **Scraper** → asset-data-full.json
2. **Generator** → DOC-10-00 (Intake)
3. **Generator** → DOC-10-00-A (Provider QA) + **Provider-Token**
4. **Email** → Provider erhält Link: `h2trading.at/provider/confirm?token=abc123`
5. **Provider** → Füllt fehlende Felder aus, bestätigt
6. **System** → Speichert Änderungen, committet zu GitHub, sendet Bestätigungs-Mail
7. **Generator** → DOC-10-01 (Exposé) mit verifizierten Daten

**Effort:**
- Integration + Testing: **10h**

---

## Total Effort Estimation

| Component | MVP | Full |
|---|---|---|
| **Provider-Portal** | 10h | 18h |
| **Admin Dashboard** | - | 20h |
| **Integration** | - | 4h |
| **Testing & Polish** | - | 6h |
| **TOTAL** | **10h** | **48h** |

---

## Implementation Plan (Option A - Recommended)

### Phase 0: Prerequisites (IN PROGRESS)
- ✅ Required Fields Taxonomie finalisieren (HARD/SOFT classification)
- ✅ Batch-Regeneration (51 Assets mit final generator)
- ✅ 1-2 manuelle Provider-Tests (validate workflow)

**Status:** Waiting on Required Fields Review (53 fields, 42 TBD)

---

### Phase 1: Provider-Portal MVP (10h)

**Milestone:** Provider können Anbieteranfragen bestätigen

**Tasks:**
1. Token-Generator (unique per asset) - **2h**
2. Provider-Portal Backend (Express) - **2h**
3. DOC-10-00-A Rendering (HTML) - **2h**
4. Confirm-Flow (checkboxes → save) - **2h**
5. Mail-Trigger (Brevo API) - **1h**
6. Basic UI (PRJ-04 Design) - **3h**

**Deliverables:**
- `/provider/confirm?token=xxx` endpoint
- Email template (Provider-Einladung)
- Confirmation page (Success)

---

### Phase 2: Provider-Portal Full (8h)

**Milestone:** Provider können fehlende Pflichtfelder ausfüllen

**Tasks:**
1. Form-Generator (dynamic from required-fields.v2.json) - **4h**
2. Validation + Save - **2h**
3. Diff-Report (was changed) - **2h**

**Deliverables:**
- Dynamic forms für fehlende Felder
- Validation messages (PRJ-04 styled)
- Diff-Report in Confirmation-Mail

---

### Phase 3: Admin Dashboard (20h)

**Milestone:** Interne Verwaltung von Klassen + Pflichtfeldern

**Tasks:**
1. Klassen-Verwaltung (CRUD) - **4h**
2. Pflichtfelder-Editor (UI) - **6h**
3. Master-Template-Editor (Markdown) - **4h**
4. Batch-Actions (trigger scripts) - **2h**
5. UI/UX (PRJ-04) - **4h**

**Deliverables:**
- `/admin/classes` (CRUD interface)
- `/admin/required-fields` (HARD/SOFT editor)
- `/admin/templates` (Markdown editor + preview)
- `/admin/batch` (regenerate button)

---

### Phase 4: Integration & Testing (10h)

**Tasks:**
1. End-to-End Workflow - **4h**
2. Email Templates (Provider + Confirmation) - **2h**
3. Error Handling + Edge Cases - **2h**
4. Documentation - **2h**

**Deliverables:**
- Full workflow tested (Scraper → Portal → Verified → Exposé)
- Email templates (DE + EN)
- README.md (how to use portal)

---

## Risks & Mitigations

### Risk 1: Taxonomie ändert sich
**Problem:** Wenn HARD/SOFT Felder sich ändern, müssen Portal-Forms angepasst werden  
**Mitigation:** Phase 0 abwarten (Taxonomie finalisiert), dann bauen

### Risk 2: Provider adoptieren nicht
**Problem:** Provider bevorzugen weiterhin E-Mail  
**Mitigation:** A/B Test (50% Portal, 50% E-Mail), ROI messen

### Risk 3: Security (Token-Leaking)
**Problem:** Provider-Links könnten weitergegeben werden  
**Mitigation:** Tokens einmalig nutzbar (nach Confirm = invalid), IP-Check optional

---

## Alternatives Considered

### Alternative 1: Interaktive PDF-Forms
**Konzept:** DOC-10-00-A als PDF mit Formularfeldern  
**Vorteil:** 2h Entwicklung, sofort nutzbar  
**Nachteil:** Kein Auto-Mail, kein Audit-Trail, weniger elegant  
**Entscheidung:** ❌ Nicht gewählt (Portal ist langfristig besser)

### Alternative 2: Google Forms / Typeform
**Konzept:** Externe Form-Tools nutzen  
**Vorteil:** 0h Entwicklung  
**Nachteil:** Kein PRJ-04 Branding, manuelle Integration  
**Entscheidung:** ❌ Nicht gewählt (keine Kontrolle über Workflow)

---

## Success Metrics

**MVP Success:**
- ✅ 10+ Assets via Portal verifiziert
- ✅ <5 Min durchschnittliche Provider-Zeit
- ✅ 0 manuelle Nachfragen nötig

**Full Success:**
- ✅ 90% Provider-Adoption (vs E-Mail)
- ✅ 50% fehlende Pflichtfelder via Portal ergänzt
- ✅ <10h/Monat manuelle Arbeit (vs 25h vorher)

---

## Dependencies

**Blockers:**
- Required Fields Taxonomie muss finalisiert sein (HARD/SOFT)
- Batch-Regeneration muss complete sein (51 Assets)
- 1-2 manuelle Provider-Tests müssen validieren dass Workflow funktioniert

**Nice-to-Have:**
- Brevo Email-Templates (DE + EN)
- PRJ-04 UI-Components library (für schnelleres Styling)

---

## Questions to Answer

1. **Token-Expiry:** Wie lange sind Provider-Links gültig? (7 Tage? 30 Tage? Unlimited?)
2. **Multi-Language:** Portal in DE + EN? (Provider könnten international sein)
3. **Notification:** Soll H2T benachrichtigt werden wenn Provider Form ausfüllt? (Telegram? Email?)
4. **Re-Open:** Können Provider nach Confirm nochmal editieren? (oder locked?)
5. **Analytics:** Tracking nutzen (Google Analytics) oder Privacy-First (keine Tracking)?

---

## Next Steps (When Ready)

1. **Review this document** with Command (Stephan + Elias)
2. **Prioritize:** Confirm Phase 0 complete (Taxonomie + Batch-Regen)
3. **Kickoff:** Create GitHub Project Board for tracking
4. **Design:** Wireframes für Provider-Portal (Figma? Low-fi Sketch?)
5. **Develop:** Phase 1 MVP (10h sprint)

---

## References

**Related Documents:**
- `/docs/roadmap/` (this folder)
- `required-fields-derivation/REPORT.md` (Taxonomie)
- `MEMORY.md` (Lessons Learned: Strategic planning > tactical fixes)

**Related Issues:**
- (none yet - will be created when work starts)

**Related PRs:**
- (none yet)

---

**Status:** 💡 Idea documented, ready for later implementation  
**Owner:** Captain Kirk (OpenClaw)  
**Stakeholders:** Stephan (Command), Elias (Starfleet)
