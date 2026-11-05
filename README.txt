ORION BLACK GOLD — WEBSITE STARTER

Files:
- index.html: the app interface and local features
- manifest.webmanifest: installable web app metadata
- sw.js: basic offline caching
- icon.svg: app icon

PHONE-ONLY PUBLISHING:
1. Upload this project to a static website host that supports direct ZIP upload (for example, Cloudflare Pages Direct Upload).
2. Upload the ZIP archive or extracted project folder as the host requests.
3. Open the published HTTPS website in Chrome on Android.
4. In Chrome, tap ⋮ and choose "Add to Home screen" or "Install app".

CURRENT LIMITATIONS:
- Chat is a local command-based prototype, not connected to a live AI model.
- Tasks and memories are stored in this browser on this device.
- Voice depends on browser speech recognition support and permissions.
- Web search opens a search engine.
- Direct Android device controls and background automation are not implemented.

SECURITY:
Do not put private API keys in index.html or any browser-side JavaScript.
A real AI connection should use a secure server-side endpoint.
