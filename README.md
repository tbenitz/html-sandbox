# HTML Sandbox

A simple, local HTML playground for quickly testing HTML files that make API calls or hit CORS restrictions.

## Features

- **Paste** HTML directly into the editor
- **Upload** an `.html` file
- **Drag & drop** an HTML file onto the window
- Live preview in a sandboxed iframe (blob URL)
- Basic console capture from the preview
- Resizable editor/preview panes
- `Ctrl/Cmd + Enter` to run
- Auto-saves your last code to localStorage
- Example button with a CORS/fetch demo

## Usage

1. Open `index.html` in any modern browser (or serve it with a local server).
2. Paste, upload, or drop an HTML file.
3. Hit **Run** (or `Cmd/Ctrl+Enter`).

Because the preview runs from a `blob:` URL, it has a unique origin. This is useful for observing real CORS behavior — failed cross-origin requests will show up in the console just like they would in a normal page.

## Notes

- The iframe uses `sandbox="allow-scripts allow-modals allow-forms allow-popups allow-same-origin"`.
- Console hooking works for same-origin (blob) content; open browser DevTools on the iframe if you need more detail.
- No server required — everything runs client-side.

## License

MIT
