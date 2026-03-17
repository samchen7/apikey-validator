## API Key Validator

A lightweight web tool for checking whether your API keys are **valid, expired, or lack permissions**, using multiple large language model endpoints.

### 🚀 Quick Start

```bash
python3 -m http.server 8888
```

Open in your browser: `http://localhost:8888`

### How to Use

1. Enter the **API Key you want to test**  
2. Select the target **model**  
3. (Optional) Enter a simple prompt (e.g. “Hello”)  
4. Click **Send Request**  
5. Check the **response panel** and **error message**:
   - Normal model reply ⇒ key is valid  
   - Error like “invalid API key”, “unauthorized”, “permission denied”, “access token expired” ⇒ key is invalid or expired  

### Features

- Works with 80+ LLMs (GPT, Claude, DeepSeek, Gemini, Grok, Qwen, etc.)
- Flexible API endpoint: test keys against different compatible gateways
- Clear error surfacing: highlights common auth / permission issues
- Token management: live token count and limit checking
- Model validation: automatically validates model names

### ⚠️ Notes

- Model names must match exactly; only the listed models are supported  
- Default API endpoint: `https://marketplace.aisa.one/pg/chat/completions`  
- API Keys are only stored locally in your browser (never sent anywhere else except the configured API endpoint)  
