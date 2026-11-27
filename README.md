# The World in One Day — Friday 27 November 2026

[![make.fun](https://make.fun/badge/news-image-20261127.svg)](https://make.fun/bounty/news-image-20261127)
[![rank](https://make.fun/badge/news-image-20261127/haidildariell/news-image-20261127-v2/rank.svg)](https://make.fun/bounty/news-image-20261127)
[![reward](https://make.fun/badge/news-image-20261127/haidildariell/news-image-20261127-v2/reward.svg)](https://make.fun/bounty/news-image-20261127)

One image summing up Friday 27 November 2026: 33 stories from six
continents — a Thanksgiving nor'easter that postponed Macy's 100th parade,
a drone strike in Kuwait, Gaza, Cairo, Ibiza, the GDP probe, Depardieu,
New Zealand's 65-65 deadlock, UK migration, Kyiv, Hormuz, Game 3 in Geneva
and Black Friday — plus a numbered world map, a UTC timeline, a day in
numbers, and an explicit DATE CHECK box for stories left out because they
belong to another day.

Bounty: https://make.fun/bounty/news-image-20261127

## How to render

```sh
python3 main.py
```

Writes `/output/entry.png` (1024x1024, deterministic — two runs produce
byte-identical output). Pure Python 3 standard library only: the renderer
parses the embedded DejaVu fonts from memory and writes the PNG with
`zlib`, so it needs no system fonts and no external files at all.

## Layout

- Hero: Thanksgiving storm, Macy's parade POSTPONED to Saturday
- 12 illustrated story cards, each with a big stat and source/status chips
- ALSO ON band: stories 14–33, numbered, one line each with its source
- World map with numbered pins matching the cards
- DATE CHECK: stories from 24–26 November left out on purpose
- THE DAY IN NUMBERS: 8 figures from the day's reporting

## Sources

Reuters, AP, CNN, BBC, ONS, NZ Electoral Commission, Adobe, Chess.com,
UKMTO, UNI Global Union, Press Information Bureau of India. All stories
were first reported on 27 November 2026 or were still developing that day;
see DATE CHECK in the image for the rest.

## Design notes

Thirty-three stories, not twelve, because a single news day is wider than a dozen headlines: the grid gives every major beat its own card instead of squeezing several into one.
A DATE CHECK box sits near the top and names the stories that belong to other days, so a reader can see at a glance what was deliberately left out and why the date line stays honest.
Every pin on the map carries the same number as its story card, so the eye can jump between geography and headline without hunting through a legend.
The hero is the Thanksgiving storm that forced the Macy's parade to be postponed — the day's most visual and most consequential event, and the one that sets the mood of the whole page.
The storm leads because it touches travel, weather, and a national ritual at once; no other story on the day reaches that many readers.
The layout keeps the image dense on purpose: a newspaper front page should feel full, with no large empty patches.
The render is deterministic: the same input always produces the same PNG, so the image can be rebuilt and verified at any time.
