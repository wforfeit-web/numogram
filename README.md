# Numogram

An interactive map of the CCRU Numogram (the Decimal Labyrinth), in lime and black.

## Features

- **Reading:** tap a zone for its region, syzygy, current and gate; tap a second zone for the demon of that pair (type, mesh number, span, sum).
- **Pandemonium:** the full 45-demon matrix, coded syzygetic / chronodemon / amphidemon / xenodemon.
- **AQ:** Alphanumeric Qabbala calculator (0–9 as themselves, A=10 … Z=35) with digital reduction to a zone.
- **Gate paths:** follow gates from any zone until the path falls into a loop.
- Installable as an app (PWA) and works offline after the first visit.

## Rules implemented

| Rule | Formula |
|---|---|
| Syzygy | zone *z* pairs with 9 − *z* |
| Current | larger − smaller of the syzygy |
| Gate | digital reduction of 0 + 1 + … + *z* (Gt-*n*) |
| Regions | Warp {3,6}, Plex {0,9}, Time-Circuit {1,2,4,5,7,8} |
| Mesh number | for pair *a*::*b* (*a* > *b*): *a*(*a*−1)/2 + *b* |

## Run locally

Open `index.html` in a browser. For install/offline support, serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Publish on GitHub Pages

1. Create a new repository on GitHub and upload these files (or `git push` them).
2. Settings → Pages → Source: *Deploy from a branch* → `main` / root → Save.
3. Your app is live at `https://<username>.github.io/<repo>/`.
4. On a phone, open that link and choose **Add to Home Screen** to install it.

## Note

The Numogram originates in the writings of the Cybernetic Culture Research Unit (CCRU). This is an independent fan-made tool; demons are labeled by zone pair and mesh number.

## License

MIT
