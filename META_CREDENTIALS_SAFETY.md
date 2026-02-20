# META – Credential & Access Safety Policy (STOP RULE)

**Gültig ab:** 2026-02-19  
**Grund:** Sicherheit, Nachvollziehbarkeit, Container-Stabilität

---

## STOP: Keine Secrets im Chat
Frage **niemals** nach Zugangsdaten/Secrets (Tokens, API Keys, Passwörter, Cookies, SSH Keys, Recovery Codes).

Wenn du welche brauchst, antworte:
> „Bitte setze das Secret ausschließlich in **hPanel → Docker Manager → Environment** oder in **docker-compose.yml / .env** und starte danach den Container neu."

---

## STOP: Keine Änderungen an Secrets per Tool/Command
Du darfst **keine** Dateien/Kommandos erzeugen oder ändern, die Secrets enthalten oder verarbeiten:
- `.env`
- `openclaw.json` (wenn Secrets direkt drin sind)
- `token_*.txt`
- `auth.*`
- `config*` (wenn Secrets direkt drin sind)
- Shell-History

Auch **kein** `echo TOKEN=…` oder ähnliche Workarounds.

### Ausnahme: Git Operations
Für `git push` darfst du den Token **aus** `/data/.openclaw/secrets/token_github.txt` lesen und in der Remote-URL verwenden:
```bash
TOKEN=$(cat /data/.openclaw/secrets/token_github.txt) && git push https://$TOKEN@github.com/...
```
**Wichtig:** Token wird **nicht** in Chat/Logs ausgegeben, nur in der Command-Execution verwendet.

---

## STOP: Keine Ausgabe von Secrets
Wenn irgendwo ein Secret auftaucht (Logs, Config, Screenshots, untrusted metadata), musst du es **maskieren** und darfst es nicht wiederholen oder rekonstruieren.

---

## Erlaubter Workflow
Du darfst **nur Anweisungen geben**, wo Secrets eingetragen werden sollen:
1. hPanel → Docker Manager → Environment/Compose  
2. oder `.env`-Datei (manuell durch Nutzer)

Danach darfst du zu einem **Recreate/Restart** anleiten.

---

## Port-/URL-Regel
Verwende für Zugriff immer den **aktuell funktionierenden externen Port**.

Wenn ein Port nicht erreichbar ist, leite an:
- Port-Mapping prüfen
- Firewall-Regeln prüfen

**Nicht** einfach Ports wechseln oder Services direkt öffentlich machen.

---

## Wenn ich gegen eine STOP-Regel verstoßen soll
**Lehne ab** und nenne den sicheren Alternativschritt.

---

## Beispiel (Discord-Setup)
❌ Falsch:
```bash
echo "DISCORD_TOKEN=MTQ3N..." > /data/.openclaw/secrets/token_discord.txt
openclaw config set channels.discord.token $(cat /data/.openclaw/secrets/token_discord.txt)
```

✅ Richtig:
> „Bitte setze in hPanel → Docker Manager → Container Environment:  
> `DISCORD_TOKEN=<dein-token>`  
> und starte den Container neu. Danach konfiguriere ich OpenClaw per:  
> `openclaw config set channels.discord.tokenEnv DISCORD_TOKEN`"
