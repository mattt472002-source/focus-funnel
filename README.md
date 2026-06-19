# Focus Funnel

A tiny, single-file task triage app. Dump everything on your mind, sort each
item into **Now / Next / Never**, then enter Focus mode and work one task at a
time.

## Features

- **Brain dump** — capture tasks fast; new items land in **Next** by default.
- **Three buckets** — drag cards between **Now**, **Next**, and **Never**.
- **Focus mode** — step through your **Now** tasks one at a time, marking each
  done or skipping to the next.
- **Bulk actions** — clear the **Never** column or clear completed tasks.
- **Auto-save** — everything is stored in your browser via `localStorage`, so
  your tasks persist across reloads.

## Running it

No build step and no dependencies. Just open the file in a browser:

```sh
# from this folder
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or double-click `index.html` in your file manager.

## How it works

The entire app — HTML, CSS, and JavaScript — lives in
[`index.html`](index.html). State is kept under the `localStorage` key
`focus-funnel-v1`. Clearing your browser storage resets the board.
