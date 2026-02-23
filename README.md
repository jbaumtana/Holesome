# Great Lakes Pullover — Interactive Knitting Guide

Interactive React app with animated stitch simulations, size-specific stitch numbers, and a full construction walkthrough for the Great Lakes Pullover by Ozetta.

---

## Running with Claude Code

### 1. Install Claude Code (if you haven't)

```bash
npm install -g @anthropic-ai/claude-code
```

### 2. Navigate to this project folder

```bash
cd great-lakes-app
```

### 3. Launch Claude Code

```bash
claude
```

### 4. Ask Claude Code to run the app

Once inside Claude Code, try prompts like:

```
Install dependencies and start the dev server
```

```
Run npm install then npm start
```

Claude Code will install packages and launch the app at **http://localhost:3000**

---

## Running without Claude Code

If you just want to run it directly:

```bash
npm install
npm start
```

---

## What's inside

```
great-lakes-app/
├── public/
│   └── index.html
├── src/
│   ├── index.js       ← entry point
│   └── App.jsx        ← the full interactive guide
└── package.json
```

---

## Things to ask Claude Code

Once the app is running, you can ask Claude Code to modify it:

- `"Add a yarn calculator that estimates yardage based on size"`
- `"Add a progress tracker that saves which steps I've completed"`
- `"Make the animations faster"`
- `"Add a dark mode toggle"`
- `"Export the stitch numbers for my size as a PDF"`
- `"Add a notes section to each step"`

Claude Code can read the source, make edits, and hot-reload the changes live.

---

## Requirements

- Node.js 18+
- npm 8+
