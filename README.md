# Claude Projects

Index of all projects built with Claude.

---

## Projects

### 🎯 [Wordsmith](https://github.com/spemmaraju/hangman-game) — Hangman × Wheel of Fortune
**Runs locally on macOS** (double-click `start.command` to launch)

A brain-training word game blending classic Hangman with Wheel of Fortune mechanics. Six game types test vocabulary, general knowledge, and lateral thinking — all with a timed countdown and progressive hints.

**Features:**
- 6 game modes: Word, Phrase, Famous Quote (guess quote + author), Idiom, Country/Capital, Trivia — plus a Surprise Mix
- Adjustable countdown timer (30s – 3 min in 30s steps, default 90s)
- Auto-hints at 75%, 50%, 25% time elapsed (category → definition → letter reveal) — each costs points
- Manual hint button available at any time (−75 pts per hint)
- Classic SVG hangman drawing — 6 wrong-guess stages
- Scoring: 1000 base pts, −50 per wrong guess, time bonus on win, difficulty multiplier (1×/1.5×/2×)
- Local leaderboard saved to disk (top 20 per game type)
- Physical keyboard support — just type letters while playing
- Double-click `start.command` to start; auto-opens browser, auto-installs deps on first run

**Stack:** Python 3.12 · Flask · Vanilla HTML/CSS/JS (ES Modules) · Datamuse API · Open Trivia DB · REST Countries API · Free Dictionary API · local JSON datasets

---

### ⚡ [VocabForge](https://github.com/spemmaraju/vocab-builder) — Vocabulary Builder
**Live app:** https://spemmaraju.github.io/vocab-builder

An interactive GRE-level vocabulary builder with mnemonics, etymology, and spaced-practice quizzes.

**Features:**
- 42 pre-loaded words with vivid mnemonic stories and real etymologies
- 4 quiz types: Word→Definition, Definition→Word, Fill in the Blank, Story Time
- SVG countdown timer with progressive hints
- Word Ledger — searchable grid of all seen/looked-up words
- Look up any English word — auto-fills definition, pronunciation, and etymology (free, no API key)
- Progress saved locally in browser (localStorage)
- Works on Mac, iPhone, and iPad

**Stack:** Vanilla HTML/CSS/JS · GitHub Pages · Free Dictionary API · Wiktionary API

---

### 📓 [Stoic Journal](https://github.com/spemmaraju/stoic-journal) — Personal Stoic Journaling App
**Runs locally on macOS** (no live URL — journal entries never leave your machine)

A privacy-first journaling app that pairs your mood with a Stoic quote and a CBT-style reflection prompt, then saves your entry in a local-only SQLite database.

**Features:**
- 14 CBT mood options (anxious, sad, angry, lonely, overwhelmed, and more)
- Stoic quote + CBT prompt tailored to your mood on every open
- Three quote sources: Free (Quotable.io), Claude (Anthropic), or ChatGPT (OpenAI) — switchable via toggle
- Journal entries stored in local SQLite only — never transmitted externally
- Right-panel entry history showing mood and date (no full text exposed)
- Click any past entry to read it in full, or delete it permanently
- AI provider privacy: only the mood word is ever sent to external APIs; journal content stays local

**Stack:** Python 3.12 · FastAPI · SQLite · SQLAlchemy · Vanilla HTML/CSS/JS · Anthropic API · OpenAI API · Quotable.io

---

## Planned / In Progress

- **Phase 2:** Cross-device sync via GitHub Gist
- **Phase 3:** Kindle vocabulary.db import — pull words you looked up while reading into VocabForge
- **Phase 4:** iOS Shortcut for one-tap word addition
