# Cuaview

https://github.com/user-attachments/assets/fe1054bc-1618-466c-85c1-d150fc675e11

> **Note:** Nov 7 release artifacts are labeled "Archon Desktop" — same product, renamed to Cuaview.

##  Download: https://github.com/sdan/cuaview/releases/tag/v0.1.0

You can either run it locally via ollama(you will need to pre-fetch qwen3-vl:4b) or run it via openrouter with your api key. Its been tested on qwen3 235b but given we use a standard computer-use function call it should be good with other models.

#### Install

1. Open DMG, drag app to Applications
2. Grant Accessibility + Screen Recording permissions on first run

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
```

Restart after config changes.
