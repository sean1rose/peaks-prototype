# Peaks.js Interactive Segment Prototype

A single-page prototype demonstrating click-and-drag segment creation and real-time draggable segment edges using [Peaks.js](https://github.com/bbc/peaks.js).

## Features

- **Click-and-drag segment creation** — drag on the zoomview waveform to create segments
- **Draggable segment handles** — resize segment boundaries in real-time
- **Two audio modes**:
  - Ambient Tone — blank canvas for creating segments
  - Speech Sample — includes 3 pre-existing editable segments
- **Fully self-contained** — audio is generated synthetically via Web Audio API, no external files needed

## Running Locally

The prototype requires a local HTTP server (Web Audio API doesn't work with `file://` URLs).

### Option 1: Python (built-in)

```bash
cd /path/to/peaks-prototype
python3 -m http.server 8080
```

Then open http://localhost:8080

### Option 2: Node.js

```bash
npx serve .
```

### Option 3: PHP

```bash
php -S localhost:8080
```

## Usage

1. Select an audio file using the radio buttons
2. Click and drag horizontally on the top waveform (zoomview) to create a segment
3. Drag the segment handles to adjust boundaries
4. Use Play/Pause and Zoom controls as needed

## Dependencies

All loaded via CDN (no installation required):
- [Peaks.js v3](https://github.com/bbc/peaks.js)
- [Konva.js v9](https://konvajs.org/)
