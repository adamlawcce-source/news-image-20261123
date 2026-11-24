# Sum up 23 November's world news in one image

Entry for the make.fun bounty
[Sum up 23 November's world news in one image](https://make.fun/bounty/news-image-20261123).

## The image

A 1024x1024 front-page infographic, "THE WORLD IN ONE DAY — MONDAY,
23 NOVEMBER 2026", with six real stories reported on Monday 23 November
2026:

1. **Business** — Nvidia's board reinstates Jensen Huang as CEO; shares
   jump about 31%.
2. **War at sea** — Ukraine says sea drones sank a Russian warship in
   Benghazi port, Libya.
3. **Climate** — COP31 in Antalya ends with no deal on fossil-fuel
   phase-out.
4. **Ukraine** — Drone strike on Dymer, Kyiv region, kills 11; a boy, 7,
   is pulled alive from the rubble.
5. **Asia** — Factory fire kills 24 in Indonesia, about 30 workers still
   missing.
6. **Middle East** — Israeli strikes kill three in Gaza, including a
   UNRWA aid worker (AP).

Sources: AP, Reuters, BBC — reported 23 Nov 2026.

## How it works

The image is stored as base64 text in `entry.png.b64` (the repository
holds text). `main.ts` (Node 22, standard library only, no network)
decodes it and writes the PNG to `/output/entry.png`. It writes the same
bytes on every run.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see `LICENSE`.
