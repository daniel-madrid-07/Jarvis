<div align="center">

# Jarvis

**A voice-controlled AI butler for Windows, inspired by Iron Man's Jarvis.**

</div>

---

## What it does

Jarvis listens for a wake word, transcribes speech in real time on the GPU, understands what you
want via Claude, and talks back — while controlling apps, windows, Spotify, timers, and system
settings hands-free, in English or Spanish.

## Features

- **Voice control** — wake word detection, real-time GPU transcription (Whisper), natural language understanding (Claude), text-to-speech replies, and interrupt handling mid-speech
- **App & window management** — open/close apps by voice, move windows across monitors, auto-discovers your shortcuts
- **Spotify integration** — play songs, playlists, or artists by voice search; full playback control
- **System control** — shutdown/restart/lock, volume, brightness, screenshots, clipboard, run shell commands
- **Timers, reminders & memory** — set/cancel timers and reminders, remember and recall facts across sessions
- **Advanced controls** — screen reading via OCR (Claude vision), mouse/keyboard automation, gaming mode (auto-closes distracting apps)

## Installation / Usage

```bash
git clone <repo-url>
cd Jarvis
pip install -r requirements.txt
python main.py
```

Requires Python 3.10+, a microphone, and API keys in `.env` (Anthropic, optionally Spotify) — full
setup guide in [SETUP.md](SETUP.md). Voice command examples, configuration, architecture,
performance notes and troubleshooting: **[docs/USAGE.md](docs/USAGE.md)**.

## Tech stack

Python, [Claude](https://claude.ai) (Anthropic API) for language understanding and screen OCR, [Whisper](https://openai.com/research/whisper) (faster-whisper, GPU-accelerated) for speech-to-text, [Edge TTS](https://github.com/rany2/edge-tts), [Spotify API](https://developer.spotify.com) (spotipy), [OpenWakeword](https://github.com/dscripka/openWakeWord)

## License

See [LICENSE](LICENSE).
