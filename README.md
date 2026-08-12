# Birthday Celebration Website for Aditi 🎂✨

A warm, intimate, single-file birthday celebration website crafted for **Aditi**.

---

## 🚀 How to Run Locally

You can launch and preview the website on local host using any of the following methods:

### Option 1: Using `npm start` (Recommended)
In this directory, open a terminal and run:
```bash
npm start
```
Then open `http://localhost:3000` in your web browser.

### Option 2: Using Python Simple HTTP Server
If Python is installed:
```bash
python -m http.server 3000
```
Then open `http://localhost:3000`.

---

## 🎨 Personalizing the Content

Personalizing the site for Aditi is quick and easy! You can edit the top-level **`CONFIG`** object in `index.html` or update the marked HTML comments directly.

### 1. Centralized Configuration in JavaScript
Open `index.html` and edit the `CONFIG` object located at the start of the `<script>` tag:

```js
const CONFIG = {
  friendName: "Aditi",
  authorName: "Aditya",
  heroTitle: "Happy Birthday Aditi!",
  heroSubtitle: "A little corner of the internet saved just for memories...",
  cakeWishToast: "Wish made! May every single dream of yours take flight this year!",

  // Interactive Surprise Gift Boxes & Wishes:
  giftSurprises: [
    { tag: "Surprise #1", title: "A Lifetime of Laughter", icon: "🎁", message: "..." },
    { tag: "Surprise #2", title: "Unconditional Warmth", icon: "🎀", message: "..." },
    { tag: "Surprise #3", title: "Infinite Success & Peace", icon: "✨", message: "..." },
    { tag: "Surprise #4", title: "Forever Bond", icon: "💖", message: "..." }
  ],

  // Heartfelt Letter:
  letterMessage: `Dear Aditi,\n\nHappy Birthday! ...`,

  audioPath: "assets/music.mp3"
};
```

### 2. Replacing Background Music
Place your favorite background song (e.g., `music.mp3`) inside an `assets` folder or in the same directory, and update:
- `<audio id="bg-music" loop src="music.mp3"></audio>`

*Note: If no audio file is provided, the website automatically falls back to built-in warm ambient synthesized chimes using Web Audio API!*

---

## 💖 Features
- **Hero Intro**: Floating fireflies particle background canvas & warm script typography.
- **Interactive SVG Cake**: Click on each candle flame to extinguish it with realistic smoke puffs; extinguishing all candles unlocks a sparkle burst & toast wish.
- **Chat Bubble Memories**: Alternating left/right speech thread with scroll animations.
- **School Days Timeline**: Vertical timeline with connecting line progress.
- **Heartfelt Letter**: Elegant paper-style card with wax seal accent.
- **Floating Audio Engine**: Equalizer button with mute/unmute & Web Audio API fallback.
