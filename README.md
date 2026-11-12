# Sinhala Subtitle Studio

A browser app that makes Sinhala subtitles for a video or audio file.

- **Generate**: Whisper runs in the browser (free and private), or the Gemini API (you supply a free key) gives better Sinhala accuracy and can translate speech in another language into Sinhala.
- **Edit**: change the text and timings while the video plays, merge or delete lines, shift every timing at once, or import an existing `.srt`.
- **Export**: `.srt`, `.vtt` or plain text, all UTF-8.
- **Burn in**: make a new video with the Sinhala subtitles drawn on it (MP4 or WebM).

It is one static file, `index.html`, with no server code. Host it anywhere that serves static files (GitHub Pages, Netlify, Cloudflare Pages), or run it locally:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000 in Chrome or Edge. Chrome or Edge on a computer works best, because WebGPU makes Whisper faster and their MP4 recording is used for burn-in.
