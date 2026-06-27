# Common Grounds Screen Displays

Each **display set is a self-contained folder** with its own `index.html`,
`left.html`, and `right.html`. You can deploy one folder by itself, or keep many
folders in one repo and open whichever set you want. Open each page fullscreen on
its matching TV; together they read as one continuous image across both screens.
Pages loop forever and stay sharp at 4K.

```
/                      ← optional landing page listing every set (index.html)
  index.html
  common-grounds/      ← a self-contained set — deployable on its own
    index.html         ← this set's picker (left / right)
    left.html          ← left TV  (church logo)
    right.html         ← right TV ("Common Grounds")
```

## Option A — deploy ONE set (simplest)

Put just the chosen folder's contents in a repo.

1. Create a repo at https://github.com/new (Public), e.g. `common-grounds-display`.
2. **Add file → Upload files**, drag in the 3 files from `common-grounds/`
   (`index.html`, `left.html`, `right.html`). Commit.
3. **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save.**
4. After ~1 min, live at `https://YOUR-USERNAME.github.io/common-grounds-display/`:
   - Left:  `…/left.html`
   - Right: `…/right.html`

## Option B — keep ALL sets in one repo, pick a folder

Upload the whole `deploy` folder. Then each set lives under its folder name:

- Set picker: `https://YOUR-USERNAME.github.io/REPO/common-grounds/`
- Left:  `https://YOUR-USERNAME.github.io/REPO/common-grounds/left.html`
- Right: `https://YOUR-USERNAME.github.io/REPO/common-grounds/right.html`

The root `index.html` lists every set; each set's own `index.html` links to its
left/right pages.

## Put them on the screens (AbleSign)

1. Open the screen's playlist → **WEBSITES** tab.
2. Left TV → that set's `left.html` URL. Right TV → its `right.html` URL.
3. Set duration to loop — the page animates on its own.

## Adding a NEW set later

1. Duplicate the `common-grounds` folder, rename it (e.g. `fall-special/`).
2. Replace its `left.html` / `right.html`, and update the title in its `index.html`.
3. (Option B only) Add a matching card to the root `index.html`.
4. Commit — GitHub Pages redeploys automatically.

When you want a new set built, just ask — I'll generate the folder ready to drop in.
