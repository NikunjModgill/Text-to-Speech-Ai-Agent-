# Text-to-Speech-Ai-Agent-

### Node Summary

| Node | Purpose |
|------|---------|
| **Chat Trigger** | Starts the workflow on incoming chat message |
| **AI Agent** | Rewrites input text into short meaningful content |
| **Google Gemini Model** | LLM used by the agent |
| **HTTP Request (TTS)** | Sends AI text to TTS endpoint |
| **HTTP Request 1** | Polls TTS event status |
| **AI Agent 1** | Extracts only the audio URL from event response |
| **Gemini Model 1** | Supports the extraction logic |
| **HTTP Request 2** | Downloads the audio file |
| **JS Code Node** | Final JSON parsing for clean audio URL |

---

## 🔧 Setup Instructions

### 1. Import Workflow into n8n
- Go to **n8n → Workflows → Import**  
- Upload `Text-to-Speech-AI-Agent.json`

### 2. Insert Your API Keys
This workflow requires:
- Google Gemini API key  
- (Optional) Your own TTS API endpoint if you replace the demo one  

In the JSON:
