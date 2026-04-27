# 📜 The Scroll of Truth

An infinite vertical-scrolling web application displaying profound, uncomfortable truths about modern life, society, and technology. The scroll features a brutalist, ancient parchment aesthetic combined with procedural generative AI.

## ✨ Features
- **Infinite Scroll Engine**: As you reach the bottom of the feed, the application automatically uses Anthropic's `Claude 3 Haiku` API to generate new, profound truths on the fly.
- **Oracle Moderation**: Users can contribute their own truths via the modal. Before being added to the feed, the truth is evaluated by Claude to ensure it is a genuine observation and not offensive or cliché.
- **Dynamic Upvote/Downvote System**: Truths that reach a negative vote threshold are dynamically blurred out and marked as "Disputed". Truths with high upvotes receive a "Too Real" badge.
- **Procedural Ambience**: Features a native Web Audio API soundscape, including a barely audible 40Hz drone and randomized detuned bell tolls.
- **Zero Database**: All upvotes and custom submissions are stored locally on the user's device via `localStorage`.

## 🚀 Getting Started
Open `index.html` in your browser, or serve locally:
```bash
python -m http.server 8080
```
*Note: To unlock the infinite scroll and moderation features, you must supply your own Anthropic API key via the initial gateway screen.*

## 🛠️ Tech Stack
- **HTML5 & CSS3**: SVG noise filters, `writing-mode` vertical text, sticky positioning, and brutalist UI patterns.
- **Vanilla JavaScript**: State management and `IntersectionObserver` logic.
- **Anthropic API**: Real-time generative text and moderation via REST fetch.
- **Web Audio API**: Sub-bass synthesis and scheduled event playback.

---
*Built as part of the VishwaNova Weboreel Hackathon.*
