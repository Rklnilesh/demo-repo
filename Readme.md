# Happy Birthday, My Sunflower

A one-page birthday letter under a clear night sky. Stars twinkle overhead, a
shooting star crosses now and then, and the two of you sit on the hill watching
it. Below the sky: the letter, the song, and her photo.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Make it yours

1. **Her photo.** Save it in this folder as `us.jpg`. Until then the frame shows
   a soft placeholder instead of a broken image.
2. **The song.** Put your own copy of *Khat* at `assets/khat.mp3`. It fades in as
   real background music the moment she taps "tap to begin", and loops. Without
   that file the page falls back to the Spotify player, which autoplays because
   the tap counts as the gesture browsers require.
3. **Her name.** Swap "my sunflower" for it anywhere in `index.html`.
4. **A different recording.** Change the `TRACK` id in the script to any Spotify
   track id.

## Why the "tap to begin" screen

Browsers refuse to start audio until someone interacts with the page. The
overlay turns her first tap into that permission, so the song begins with the
letter instead of needing a second press.

## Files

- `index.html` — the whole page, self-contained apart from the fonts and the song
- `assets/` — where the music file goes
