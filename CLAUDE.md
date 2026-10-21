# Project notes

## watermarks-remover skills

`.claude/skills/remove-ai-marks` needs its HTTP service running. If
`curl -sf http://127.0.0.1:8765/health` fails, start it in the background with:

```bash
python3 watermarks-remover/service/scripts/server.py --host 127.0.0.1 --port 8765
```

`.claude/skills/clean-user-facing-text` runs on its own and needs no service.
