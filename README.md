# 🎙 LiveTranscribe

Trascrizione e traduzione simultanea **da inglese a italiano** in tempo reale, direttamente nel browser.

L'app ascolta l'audio in inglese tramite il microfono, lo trascrive con il riconoscimento vocale del browser e lo traduce istantaneamente in italiano usando l'API di Google Gemini. Pensata per riunioni, conferenze, lezioni e meeting online.

---

## ✨ Funzionalità

- **Trascrizione vocale in tempo reale** dell'inglese parlato
- **Traduzione automatica in italiano** frase per frase
- **Doppia visualizzazione**: testo originale inglese + traduzione italiana
- **Salvataggio in file `.txt`** con timestamp, manuale o automatico (ogni 1–10 minuti)
- **Versione mobile installabile** sulla schermata Home (PWA)
- **Schermo sempre acceso** durante la trascrizione su telefono
- **Selettore del microfono** per scegliere la sorgente audio
- **Rilevamento automatico del modello** Gemini disponibile sulla tua chiave
- **Retry automatico** in caso di limiti temporanei dell'API

---

## 🚀 Come si usa

1. Apri l'app (link di GitHub Pages)
2. Inserisci la tua **Gemini API key** (gratuita — vedi sotto)
3. Premi **Rileva modelli** e, su mobile, **Rileva microfoni**
4. Premi **Avvia** e fai arrivare l'audio inglese al microfono
5. Leggi la traduzione in italiano in tempo reale
6. A fine sessione, salva il file `.txt` con tutta la trascrizione

---

## 🔑 Ottenere la API key gratuita

1. Vai su [aistudio.google.com](https://aistudio.google.com)
2. Clicca su **Get API Key** → **Create API key**
3. Copia la chiave (inizia con `AIza...`) e incollala nell'app

Il piano gratuito di Google è più che sufficiente per l'uso normale. Nessuna carta di credito richiesta.

---

## 🎧 Catturare l'audio di una riunione (PC)

Il microfono del computer capta l'audio in arrivo dagli altoparlanti, ma per una qualità ottimale conviene instradare l'audio direttamente nel browser con un cavo audio virtuale gratuito come [VB-Cable](https://vb-audio.com/Cable/).

Schema consigliato con **VB-Cable A+B**:

| Componente | Impostazione |
|---|---|
| App riunione (es. Teams) — Altoparlante | `CABLE-A Input` |
| App riunione — Microfono | il tuo microfono fisico |
| Browser — Microfono | `CABLE-A Output` |
| `CABLE-A Output` → "Ascolta il dispositivo" | i tuoi altoparlanti reali |

In questo modo senti l'audio dalle casse **e** il browser lo trascrive contemporaneamente.

---

## 📱 Versione mobile (Android)

L'app è installabile come PWA: aprila in **Chrome su Android**, poi menu → **Aggiungi a schermata Home**.

Scenari supportati su telefono:

| Scenario | Funziona |
|---|---|
| Riunione o lezione **in presenza** | ✅ |
| Riunione su PC, telefono che ascolta l'audio | ✅ |
| Chiamata sullo **stesso telefono** | ❌ (il microfono è occupato dall'app della chiamata) |

---

## ⚙️ Requisiti

- **Browser**: Chrome, Edge o Brave (il riconoscimento vocale **non** è supportato da Firefox e Safari)
- **Connessione HTTPS**: necessaria per l'accesso al microfono (GitHub Pages la fornisce automaticamente)
- Una **Gemini API key** valida

---

## 🛠 Tecnologie

- **Web Speech API** per il riconoscimento vocale
- **Google Gemini API** per la traduzione
- HTML, CSS e JavaScript puri — nessuna dipendenza, un solo file

---

## 📄 Note

La qualità della traduzione dipende dalla qualità del riconoscimento vocale del browser: audio pulito, volume adeguato e una buona pronuncia migliorano sensibilmente i risultati. Termini molto tecnici e nomi propri restano i più difficili da riconoscere.

---

## 📜 Licenza

Progetto personale a uso libero.
