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
<!-- ORION MUSIC CENTER -->
<section id="orion-music-center">
  <div class="orion-music-card">
    <h2>🎵 ORION MUSIC CENTER</h2>
    <p>Your personal music command center.</p>

    <input
      id="orionMusicSearch"
      type="text"
      placeholder="Search for music..."
    />

    <button onclick="orionSearchMusic()">
      SEARCH MUSIC
    </button>

    <button onclick="window.open('https://open.spotify.com/', '_blank')">
      OPEN SPOTIFY
    </button>

    <button onclick="window.open('https://music.youtube.com/', '_blank')">
      YOUTUBE MUSIC
    </button>

    <p id="orionMusicStatus">ORION MUSIC SYSTEM READY</p>
  </div>
</section>
  </body>
<style>
#orion-music-center {
  padding: 30px 15px;
  text-align: center;
}

.orion-music-card {
  background: #080808;
  border: 2px solid #d4af37;
  border-radius: 18px;
  padding: 25px;
  color: #d4af37;
  max-width: 500px;
  margin: auto;
  box-shadow: 0 0 20px #d4af3744;
}

.orion-music-card h2 {
  color: #d4af37;
}

.orion-music-card input {
  width: 90%;
  padding: 12px;
  margin: 12px 0;
  border: 1px solid #d4af37;
  border-radius: 8px;
  background: #151515;
  color: white;
}

.orion-music-card button {
  background: #d4af37;
  color: black;
  border: none;
  padding: 12px 18px;
  margin: 6px;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
}

#orionMusicStatus {
  margin-top: 18px;
  color: #d4af37;
}
</style>

<script>
function orionSearchMusic() {
  const search = document.getElementById("orionMusicSearch").value.trim();

  if (!search) {
    document.getElementById("orionMusicStatus").textContent =
      "ENTER A SONG OR ARTIST, COMMANDER.";
    return;
  }

  document.getElementById("orionMusicStatus").textContent =
    "SEARCHING MUSIC DATABASE...";

  window.open(
    "https://music.youtube.com/search?q=" + encodeURIComponent(search),
    "_blank"
  );
}
</script> </body>

