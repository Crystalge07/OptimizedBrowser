# OptimizedBrowser

OptimizedBrowser is a Chrome extension project focused on improving tab navigation with an Arc/Zen-style vertical tabs experience.

The main extension source lives in `vertical-tabs/`.

## What It Includes

- Vertical tab list in the Chrome side panel
- Real-time tab sync (create/update/remove/move/activate)
- Tab search by title or URL with quick Enter-to-open
- Quick tab switching across windows (focuses the right window)
- Pinned tabs support (with pin/unpin drag zones)
- Drag and drop tab management (reorder + move tabs into spaces)
- Domain grouping with collapsible groups for cleaner tab lists
- Right-click tab context menu (copy link, reload, mute/unmute, pin/unpin, close)
- Reading list ("save for later") with restore and remove controls
- Stale tab prompts for inactive tabs with one-click bulk close
- Custom Spaces for tab organization (create/edit/delete, color + emoji icon)
- Space switching via click, touch gestures, and horizontal trackpad scroll
- Custom new tab page
- New tab unified search across open tabs, bookmarks, and history
- Smart navigation input (URL detection and fallback web search)
- Keyboard-first new tab UX (`Ctrl/Cmd + K`, arrow navigation, Enter)
- New tab highlights for pinned tabs
- New tab quick-access sections (Bookmarks + configurable second column)
- Second-column modes for recent downloads, frequent tabs/top sites, or recent tabs
- Background service worker for tab management

## Project Layout

```text
OptimizedBrowser/
├── README.md
└── vertical-tabs/            # Main Chrome extension app
    ├── src/
    ├── public/
    ├── manifest.json
    └── package.json
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm
- Google Chrome

### Install Dependencies

```bash
cd vertical-tabs
npm install
```

### Run in Development

```bash
cd vertical-tabs
npm run dev
```

### Build for Production

```bash
cd vertical-tabs
npm run build
```

## Load Extension in Chrome

1. Open `chrome://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked**
4. Select the `vertical-tabs/dist` folder after building

## Useful Scripts (from `vertical-tabs/`)

- `npm run dev` - start Vite dev server
- `npm run build` - create production build
- `npm run preview` - preview production build
- `npm run watch` - build in watch mode

## Tech Stack

- React
- TypeScript
- Vite
- CRXJS
- Tailwind CSS