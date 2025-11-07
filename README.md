# Cuaview



https://github.com/user-attachments/assets/fe1054bc-1618-466c-85c1-d150fc675e11



macOS builds for computer control via vision models.

> **Note:** Nov 7 release artifacts are labeled "Archon Desktop" — same product, renamed to Cuaview.

## Builds

**ollama**: Local inference via Ollama (`qwen3-vl:4b`)
**openrouter**: Cloud inference via OpenRouter API

## Install

1. Open DMG, drag app to Applications
2. Grant Accessibility + Screen Recording permissions on first run

## Configure

**Ollama:**
```bash
ollama pull qwen3-vl:4b
ollama serve
```

**OpenRouter:**
```bash
mkdir -p ~/Library/"Application Support"/"Archon Desktop"
cat > ~/Library/"Application Support"/"Archon Desktop"/user.env <<EOF
MODEL_PROVIDER=openrouter
OPENROUTER_MODEL=qwen/qwen3-vl-235b-a22b-thinking
OPENROUTER_API_KEY=sk-or-...
EOF
```

Restart after config changes.
