# Collaborate Music Productions website

Website for collaboratemusic.com. It needs no build step: `index.html` plus `img/` and `audio/`.

- **Edit:** change the text in `index.html`. Posters are in `img/` at 500×750 px.
- **Preview locally:** `python3 -m http.server` inside this folder, then open http://localhost:8000.
- **Hosting:** GitHub Pages from the `main` branch (root), on the custom domain in `CNAME`. Every push to `main` goes live in a minute or two.
- **DNS (GoDaddy):** `@` A records 185.199.108.153 / .109.153 / .110.153 / .111.153 and `www` CNAME `mayadex853.github.io`. MX/TXT records are for Microsoft 365 email; leave them alone.
- `404.html` sends old Squarespace links (e.g. /about-rover, /contact-rover) to the right section of the home page.
- **Inquiries** go to music@collaboratemusic.com. **Playlists** live in DISCO and are linked, not embedded.

## Bottom player and trailer pop-ups
- The player at the bottom streams `audio/<slug>.mp3` (128 kbps copies of the DISCO masters). Artwork lives in `img/art/<slug>.jpg`.
- Track names, artists, "Heard in" credits and waveforms are in the `TRACKS` list in the script at the end of `index.html`. To add a track, drop the MP3 and artwork in, then add one entry there.
- Any element with `data-play="<slug>"` plays that track. Any element with `data-video="yt:<YouTube id>"` or `data-video="vm:<Vimeo id>"` opens that video in the pop-up.
- The gold emblem (`img/emblem.png`) is used in the opening section, the contact section and the favicon.
