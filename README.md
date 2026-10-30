# longway-bench-assets

Mirrors of CC0 asset libraries that LongWay benchmark sandboxes download while they set up a task.
Nothing here is original work; every file is redistributed unchanged under its own license.

## Kenney library (release `kenney-library-2026-10-19`)

The 157 Kenney packs that GameCraft-Bench's `scripts/catalog.json`
([FreedomIntelligence/gamecraft-bench](https://github.com/FreedomIntelligence/gamecraft-bench)) lists, as its
`fetch_assets.py` unpacks them under `/workspace/assets/library/<category>/<pack>/`.
Fetched 2026-10-19. One archive per category:

| Archive | Packs | Files |
|---|---|---|
| `kenney-library-2d.tar.gz` | 2D | 53 584 |
| `kenney-library-audio.tar.gz` | Audio | 786 |
| `kenney-library-textures.tar.gz` | Textures | 1 119 |

`SHA256SUMS` lists each archive's sha256. Extract each into the library root:

```sh
tar xzf kenney-library-2d.tar.gz -C /workspace/assets/library
```

**Why a mirror.** The catalog's download URLs now redirect to kenney.nl's asset pages, and kenney.nl
refuses some sandbox networks (HTTP 403), so a sandbox cannot fetch the packs from the source.

**License.** All assets are by Kenney ([kenney.nl](https://kenney.nl)) and released under
[Creative Commons Zero (CC0 1.0)](http://creativecommons.org/publicdomain/zero/1.0/). Each pack keeps its own
`License.txt`; `isometric-roads` and `isometric-roads-water` ship without one and fall under Kenney's site-wide
CC0 terms. Credit to Kenney is appreciated, not required.
