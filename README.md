# Graphing Calculator

A simple, lightweight graphing calculator. Plot up to six functions, drag sliders for variables like `a` and `b`, and pick a theme (Auto, Paper, Midnight, Forest, Graphite).

- Drag to pan, scroll or pinch to zoom, hover to trace values.
- `2x`, `3sin(x)` and `a*sin(b*x)` all work; pasted notation like `y = x²` or `\frac{1}{x}` is understood.
- The Insert function button opens a palette that inserts into the selected box.

## Run in a browser

`src/index.html` is a single self-contained file. Open it in any browser.

## Run as a desktop app

Requires Node.js 18 or newer.

```
npm install
npm start
```

## Build Windows and Linux apps

Locally (build on the OS you are targeting):

```
npm run dist:win     # NSIS installer and portable .exe
npm run dist:linux   # AppImage and .deb
```

Or let GitHub build both: push a version tag and the workflow in `.github/workflows/build.yml` builds on Windows and Ubuntu runners and attaches the files to a release.

```
git tag v1.0.0
git push origin v1.0.0
```

Before publishing, replace the placeholder name, email and username in `package.json` and `LICENSE`.

## License

MIT
