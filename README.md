# 🎙 LiveTranscribe

**🌐 Language / Lingua:** [English](#english) · [Italiano](#italiano)

---

## English

Real-time **English-to-Italian** transcription and translation, right in your browser.

LiveTranscribe listens to spoken English through your microphone, transcribes it with the browser's speech recognition, and instantly translates it into Italian using the Google Gemini API. Built for meetings, conferences, lectures, and online calls.

### ✨ Features

- **Real-time speech transcription** of spoken English
- **Automatic Italian translation**, sentence by sentence
- **Dual view**: original English text + Italian translation
- **Save to `.txt` file** with timestamps, manual or automatic (every 1–10 minutes)
- **Installable mobile version** on your home screen (PWA)
- **Keep-screen-awake** during transcription on mobile
- **Microphone selector** to choose the audio source
- **Automatic model detection** for the Gemini models available on your key
- **Automatic retry** when the API hits temporary limits

### 🚀 How to use

1. Open the app (your GitHub Pages link)
2. Enter your **Gemini API key** (free — see below)
3. Press **Detect models** and, on mobile, **Detect microphones**
4. Press **Start** and let the English audio reach your microphone
5. Read the Italian translation in real time
6. When done, save the `.txt` file with the full transcript

### 🔑 Getting a free API key

1. Go to [aistudio.google.com](https://aistudio.google.com)
2. Click **Get API Key** → **Create API key**
3. Copy the key (starts with `AIza...`) and paste it into the app

Google's free tier is more than enough for normal use. No credit card required.

### 🎧 Capturing meeting audio (PC)

Your computer's microphone can pick up audio from the speakers, but for best quality it's better to route the audio directly into the browser using a free virtual audio cable like [VB-Cable](https://vb-audio.com/Cable/).

Recommended setup with **VB-Cable A+B**:

| Component | Setting |
|---|---|
| Meeting app (e.g. Teams) — Speaker | `CABLE-A Input` |
| Meeting app — Microphone | your physical microphone |
| Browser — Microphone | `CABLE-A Output` |
| `CABLE-A Output` → "Listen to this device" | your real speakers |

This way you hear the audio through your speakers **and** the browser transcribes it at the same time.

### 📱 Mobile version (Android)

The app is installable as a PWA: open it in **Chrome on Android**, then menu → **Add to Home screen**.

Supported scenarios on mobile:

| Scenario | Works |
|---|---|
| **In-person** meeting or lecture | ✅ |
| Meeting on a PC, phone listening to the audio | ✅ |
| Call on the **same phone** | ❌ (microphone is in use by the call app) |

### ⚙️ Requirements

- **Browser**: Chrome, Edge, or Brave (speech recognition is **not** supported by Firefox or Safari)
- **HTTPS connection**: required for microphone access (GitHub Pages provides it automatically)
- A valid **Gemini API key**

### 🛠 Tech stack

- **Web Speech API** for speech recognition
- **Google Gemini API** for translation
- Plain HTML, CSS, and JavaScript — no dependencies, single file

### 📄 Notes

Translation quality depends on how well the browser recognizes the spoken English: clean audio, adequate volume, and clear pronunciation greatly improve results. Highly technical terms and proper nouns remain the hardest to recognize.

### 📜 License

Personal project, free to use.

---

## Italiano

Trascrizione e traduzione simultanea **da inglese a italiano** in tempo reale, direttamente nel browser.

L'app ascolta l'audio in inglese tramite il microfono, lo trascrive con il riconoscimento vocale del browser e lo traduce istantaneamente in italiano usando l'API di Google Gemini. Pensata per riunioni, conferenze, lezioni e meeting online.

### ✨ Funzionalità

- **Trascrizione vocale in tempo reale** dell'inglese parlato
- **Traduzione automatica in italiano** frase per frase
- **Doppia visualizzazione**: testo originale inglese + traduzione italiana
- **Salvataggio in file `.txt`** con timestamp, manuale o automatico (ogni 1–10 minuti)
- **Versione mobile installabile** sulla schermata Home (PWA)
- **Schermo sempre acceso** durante la trascrizione su telefono
- **Selettore del microfono** per scegliere la sorgente audio
- **Rilevamento automatico del modello** Gemini disponibile sulla tua chiave
- **Retry automatico** in caso di limiti temporanei dell'API

### 🚀 Come si usa

1. Apri l'app (link di GitHub Pages)
2. Inserisci la tua **Gemini API key** (gratuita — vedi sotto)
3. Premi **Rileva modelli** e, su mobile, **Rileva microfoni**
4. Premi **Avvia** e fai arrivare l'audio inglese al microfono
5. Leggi la traduzione in italiano in tempo reale
6. A fine sessione, salva il file `.txt` con tutta la trascrizione

### 🔑 Ottenere la API key gratuita

1. Vai su [aistudio.google.com](https://aistudio.google.com)
2. Clicca su **Get API Key** → **Create API key**
3. Copia la chiave (inizia con `AIza...`) e incollala nell'app

Il piano gratuito di Google è più che sufficiente per l'uso normale. Nessuna carta di credito richiesta.

### 🎧 Catturare l'audio di una riunione (PC)

Il microfono del computer capta l'audio in arrivo dagli altoparlanti, ma per una qualità ottimale conviene instradare l'audio direttamente nel browser con un cavo audio virtuale gratuito come [VB-Cable](https://vb-audio.com/Cable/).

Schema consigliato con **VB-Cable A+B**:

| Componente | Impostazione |
|---|---|
| App riunione (es. Teams) — Altoparlante | `CABLE-A Input` |
| App riunione — Microfono | il tuo microfono fisico |
| Browser — Microfono | `CABLE-A Output` |
| `CABLE-A Output` → "Ascolta il dispositivo" | i tuoi altoparlanti reali |

In questo modo senti l'audio dalle casse **e** il browser lo trascrive contemporaneamente.

### 📱 Versione mobile (Android)

L'app è installabile come PWA: aprila in **Chrome su Android**, poi menu → **Aggiungi a schermata Home**.

Scenari supportati su telefono:

| Scenario | Funziona |
|---|---|
| Riunione o lezione **in presenza** | ✅ |
| Riunione su PC, telefono che ascolta l'audio | ✅ |
| Chiamata sullo **stesso telefono** | ❌ (il microfono è occupato dall'app della chiamata) |

### ⚙️ Requisiti

- **Browser**: Chrome, Edge o Brave (il riconoscimento vocale **non** è supportato da Firefox e Safari)
- **Connessione HTTPS**: necessaria per l'accesso al microfono (GitHub Pages la fornisce automaticamente)
- Una **Gemini API key** valida

### 🛠 Tecnologie

- **Web Speech API** per il riconoscimento vocale
- **Google Gemini API** per la traduzione
- HTML, CSS e JavaScript puri — nessuna dipendenza, un solo file

### 📄 Note

La qualità della traduzione dipende dalla qualità del riconoscimento vocale del browser: audio pulito, volume adeguato e una buona pronuncia migliorano sensibilmente i risultati. Termini molto tecnici e nomi propri restano i più difficili da riconoscere.

### 📜 Licenza

Progetto personale a uso libero.
