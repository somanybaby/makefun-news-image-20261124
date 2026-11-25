[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/somanybaby/makefun-news-image-20261124/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/somanybaby/makefun-news-image-20261124/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

# news-image-20261124 entry

One image that sums up the world news of **Tuesday 24 November 2026**, drawn
as a newspaper front page: the date in large type, the day's lead story
(Nvidia reinstates Jensen Huang; shares +31%), and five more panels —
Ukraine's sea drones sink the Russian corvette Merkury in Libya, tankers hit
mines in the Strait of Hormuz, an Israeli strike kills Hamas's security chief
in Gaza, NATO's alarm over Russia's reported nuclear satellite, and US states
suing Musk's firms over Grok's sexualised images. Every story was checked
against that day's reporting (Reuters, AP, AFP, Al Jazeera, CNN).

## How it works

`main.py` (Python 3, standard library only) contains **no embedded image
data**. The front page is drawn at run time by the program itself: a
hand-defined 5x7 bitmap font, a small word-wrapping typesetter, and a
minimal PNG writer built on `struct` and `zlib`. Running the program
renders the whole page — deep blue background, masthead, lead panel and
five story panels — pixel by pixel, then writes it out as a PNG.

## Run it

```sh
python3 main.py                        # writes /output/entry.png
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
```

The output goes to `$MAKEFUN_OUTPUT_DIR/entry.png` (default
`/output/entry.png`). The render is fully deterministic: repeated runs
produce byte-for-byte identical files.

## Output

- Format: PNG, 1024x1024, 8-bit RGB
- Size: 19376 bytes
- sha256: 6b6d696f19ed79985f72ffca05ae0742c0648da356890b77709acde4f5b3d711
