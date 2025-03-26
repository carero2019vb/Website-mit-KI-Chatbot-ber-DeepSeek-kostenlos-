# KI ChatBot mit DeepSeek über OpenRouter

Dieses Projekt enthält ein vollständiges, deployfähiges Setup:

- 🎯 **Frontend**: React (Vite-basiert, Vercel-ready)
- 🧠 **Backend**: Node.js + Express (Render-ready)
- 🔌 **KI-Integration**: DeepSeek-Modell über [OpenRouter.ai](https://openrouter.ai)

## 🔧 Setup

### 1. Frontend starten

```bash
cd frontend
npm install
npm run dev
```

### 2. Backend starten

```bash
cd backend
npm install
node index.js
```

## 🚀 Deployment

### Vercel (Frontend)
- Repo importieren
- `VITE_API_URL` in den Umgebungsvariablen auf deine Render-URL setzen

### Render (Backend)
- Neues Web Service erstellen
- Umgebungsvariable `OPENROUTER_API_KEY` setzen
- Build Command: `npm install`
- Start Command: `node index.js`

## 🧠 Prompt Engineering Hinweis

Das DeepSeek-Modell wird über die OpenRouter-API angesprochen. Die systematische Prompt-Struktur lautet:

```json
[
  { "role": "system", "content": "Du bist ein hilfreicher Assistent." },
  { "role": "user", "content": "..." }
]
```

## 🗂 Projektstruktur

```
/frontend    → React App
/backend     → Express Backend mit API-Anbindung an OpenRouter
```

---

Erstellt für Lernzwecke, Prompt Engineering und KI-Integrationen.
