# 🎤 Lyric Stream Karaoke

A lightweight and aesthetic karaoke-style web lyric streamer. Smooth line-by-line navigation, stylish transitions, and full keyboard control — all in a single HTML file.

## 🚀 Features

- ⬆️ / ⬇️ Arrow keys to scroll through lyrics
- ⇧ + ⬅️ / ➡️ to switch between songs
- Fully keyboard-controlled
- Smooth scaling and fade animation for active lines
- Background options: image, video, or gradient
- Optional grain effect overlay
- Responsive layout
- Easily extendable with new songs and themes

## 📂 Project Structure
```
lyric-stream/
├── index.html       # Main app with HTML, CSS, JS
├── README.md        # Project documentation
```
> ⚠️ No build steps required. No frameworks. No server. Just open `index.html` in any modern browser.

## 🛠 How to Run

1. Clone or download the repository:
```bash
git clone https://github.com/yourusername/lyric-stream.git
cd lyric-stream
```

2.	Open the file in your browser:
```
open index.html   # or just double-click it
```

## ⚙️ Configuration

Inside the <script> section, you can adjust basic settings:
```
const config = {
  loopLines: false,               // Enable looping lyric lines
  autoplayEnabled: false,         // Automatically scroll lyrics
  autoplayIntervalMs: 1400,       // Autoplay interval (ms)
  initialSongId: "nenavizhu"      // Initial song ID on load
};
```

## 🎵 How to Add New Songs
Inside the songs array in the JavaScript section:
```json
{
  id: "my_song_id",
  title: "Song Title",
  artist: "Artist Name",
  lines: [ "Line 1", "Line 2", "..." ],
  theme: {
    primary: "#hex",
    secondary: "#hex",
    backgroundType: "video" | "gif" | "gradient",
    backgroundMedia: "https://your-media-url.com",
    grain: true | false
  }
}
```

## 💡 Ideas for Extensions
	•	Auto-sync with audio (.lrc support)
	•	YouTube background + lyrics overlay
	•	Mobile-friendly controls
	•	Microphone input & pitch detection

## 📄 License

MIT — Free to use, modify, and share.
