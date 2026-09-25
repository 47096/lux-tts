# LuxTTS voice cloning

**Demo — clone a voice from a short sample and speak text in Colab.**

Not a client case study. A browser-only walkthrough of LuxTTS: reference audio → voice embedding → speech. GPU runtime recommended.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/47096/lux-tts/blob/main/analysis.ipynb)

---

## Run it (easy path)

1. Click **Open In Colab** above  
2. **Runtime → Change runtime type → GPU (T4)**  
3. Run all cells · upload a 5–20s WAV/MP3 · download `output.wav`  

Or locally: `analysis.ipynb` with a CUDA GPU.

---

## Five commercial use cases

| # | Use case | Who cares | Why it pays |
|---|----------|-----------|-------------|
| 1 | **Brand voice for ads** | Marketing | One talent session → unlimited spots |
| 2 | **E-learning narration** | L&D / EdTech | Course VO without studio days |
| 3 | **Product demo voiceovers** | Product marketing | Update copy without re-record |
| 4 | **IVR / voice assistant brand** | CX / ops | Consistent agent voice at scale |
| 5 | **Accessibility “listen” mode** | Product | Your UI reads itself in a familiar voice |

## Five personal use cases

| # | Use case | Why |
|---|----------|-----|
| 1 | **Podcast / YouTube VO** | Keep your voice when you can’t record |
| 2 | **Language practice** | Hear target-language sentences in a voice you know |
| 3 | **Memory keepsake** | Family voice for messages (with permission) |
| 4 | **Audiobook drafts** | Proof-listen a chapter before real narration |
| 5 | **Accessibility for you** | Long articles read aloud in a preferred voice |

---

## When to use it

- Learning **voice clone → TTS** pipelines  
- Quick prototypes for content teams  
- Teaching **consent, ethics, and limits** of cloning  

## When not to

- Impersonating people without consent  
- Production at scale without legal review (this is a demo)  

## Settings (in the notebook)

| Param | Default | Role |
|-------|---------|------|
| `rms` | 0.01 | Volume |
| `t_shift` | 0.9 | Quality vs clarity |
| `num_steps` | 4 | Quality vs speed (3–4 fast, 6+ polished) |
| `speed` | 1.0 | Rate |
| `return_smooth` | False | Smooth vs crisp |
| `ref_duration` | 10000 | How much of the sample to encode (ms) |

## Stack

[LuxTTS](https://github.com/ysharma3501/LuxTTS) · Colab GPU · `soundfile`

---

*Demo companion to product work on `mimo-reader` / `hanna` · [datafying](https://datafying.co/).*
