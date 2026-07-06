# Mea Studio website

Static landing site for Mea Studio, a flower studio in Batumi.

## Local preview

```bash
python3 -m http.server 8000
```

Open `http://127.0.0.1:8000/`.

## Netlify

Netlify can deploy this repository directly. The build settings are already in `netlify.toml`:

- Build command: `rm -rf dist && mkdir -p dist/assets && cp index.html styles.css script.js robots.txt dist/ && cp -R assets/photos dist/assets/photos`
- Publish directory: `dist`

For future edits, update `index.html`, `styles.css`, `script.js`, or files inside `assets/photos`, then commit and push to GitHub.
