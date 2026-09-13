# Happy Birthday, My Lily

A one-page birthday letter under a clear night sky. The stars hold still while
the page scrolls, and the two of you sit on the hill watching them. It opens on
that same sky with a single invitation to tap.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Put it online

The site is plain static files at the repo root, so any static host works with
no build step and no configuration.

**Vercel**

1. Go to vercel.com/new and import `Rklnilesh/demo-repo`.
2. Framework preset: **Other**. Leave build command and output directory empty.
3. Under Settings > Git, set the production branch to
   `claude/love-message-webpage-wbc8c3`, or merge that branch into `main` first
   and leave the default.
4. Deploy. The link is live in under a minute.

Add `us.jpg` and `assets/khat.mp3` before deploying, or push them afterwards.
Vercel redeploys on every push, so the live link updates on its own.

**GitHub Pages**

In the repository Settings > Pages, pick the branch and the root folder. Same
files, same result.

## Make it yours

1. **Her photo.** Save it in this folder as `us.jpg`. Until then the frame shows
   a soft placeholder instead of a broken image.
2. **The song.** Put your copy of *Khat* at `assets/khat.mp3`. It fades in when
   she taps to begin and loops quietly under the whole page. There is no visible
   player, and no link out to anywhere. If the file is missing the page simply
   stays silent.
3. **Her name.** Swap "my lilyy" for it anywhere in `index.html`.

## Why the "tap to begin" screen

Browsers refuse to start audio until someone interacts with the page. That tap
is the permission, so the music can begin with the letter. It also holds the
words back until she is ready, so the first thing she sees is just the sky and
the two of you under it.

## Files

- `index.html` — the whole page, self-contained apart from the fonts and the song
- `assets/` — where the music file goes
