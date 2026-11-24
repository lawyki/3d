# Contributing

Thanks for wanting to help. This repo is a set of standalone 3D web pages. There is no build, no package manager and no framework to learn.

## Viewing a piece

Most pages open straight from disk: double-click `<piece>/index.html`. Some browsers block WebGL textures or fonts on `file://`, so the reliable way is a tiny local server from the repo root:

```sh
python3 -m http.server 8000
# then open http://localhost:8000/vare/
```

Pieces that use three.js load version 0.160 from unpkg, so they need a network connection. Everything else is self-contained.

A desktop GPU is the target. Phones should work, but expect lower frame rates on the heavier pieces (Väre, Kehä, Microscope, Lyse).

## How the repo is laid out

- One folder per piece. The page is always `index.html`; screenshots go in `stills/`.
- A page is one file: HTML, CSS, JS and shaders inline. Fonts are either from Google Fonts or embedded as base64. Keep it that way so a piece can be copied anywhere and still run.
- `vare/src.html` is the readable source of `vare/index.html` with font placeholders (`__UNB800__` and similar) instead of the embedded fonts.
- Many pages expose small debug hooks on `window` (for example `__set(p)` to jump to a scroll position, `__noAdapt` to switch off adaptive resolution). Look near the bottom of the script.

## Making a change

1. Pick an open issue, or open one describing what you want to do.
2. Branch from `main`, keep one piece per pull request where possible.
3. Check the page in at least Chrome and Safari or Firefox, desktop and phone width (390 px). Note the GPU you tested on in the PR.
4. If the change is visual, attach a before and after screenshot. Use the piece's `stills/` folder for screenshots that should stay.
5. Don't add a build step, a bundler or new external dependencies without discussing it in an issue first.

## Style notes

- Respect `prefers-reduced-motion`: slow or stop ambient motion when it is set.
- Real DOM text for anything a person needs to read or click, even when it is drawn into the 3D scene, so screen readers and search still work.
- No tracking, analytics or third-party scripts beyond three.js and Google Fonts.

## Adding a new piece

Make a new folder, put the page at `index.html`, add a row to the table in `README.md` with a one-line description, and add at least one still.
