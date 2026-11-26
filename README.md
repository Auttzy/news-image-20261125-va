# The Wednesday Ledger — 25 November 2026

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/Auttzy/news-image-20261125-va/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/Auttzy/news-image-20261125-va/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

A newspaper front page, drawn as a single image, summing up the world's news
of Wednesday 25 November 2026.

## The image

`entry.png` is a 1024×1024 front page of a cream broadsheet called "The
Wednesday Ledger", dated Wednesday 25 November 2026. Thirty-three stories
from that day share the page, across seven regions:

- **Lead** — The US Army blows up 9,500 lb of unstable lead azide in Iowa —
  and it works: EPA monitors read 0.0 lead so far, no damage, no injuries.
- **Lead** — Asia's AI sell-off: KOSPI −6.16% to 4,697.51, Nikkei −2.78%,
  Taiex −4.80%, as tariff threats return and Tuesday's Nvidia relief rally
  evaporates.
- **Lead** — China launches Shenzhou-24 at 00:18 UTC; Muhammad Zeeshan Ali
  becomes the first Pakistani in orbit, and the first foreign astronaut
  aboard Tiangong.
- **Americas** — Wall Street whipsaws: the Nasdaq falls 4.6% intraday, then
  closes −0.62%; US PCE inflation prints 3.8% and Q3 GDP is revised to 4.3%.
  All ~30 hostages are freed as the Cartagena supermarket siege ends.
  California king tides peak at a forecast 8.5 ft.
- **Africa** — A fuel tanker overturns on Cairo's Ring Road, killing 31.
  South Africa's Ramaphosa wins his Phala Phala court battle; Kenya and DR
  Congo restore full diplomatic ties; Nigeria holds its rate at 23%.
- **Middle East** — Two more tankers are hit in the Strait of Hormuz; the
  Houthis claim attacks on Ras Tanura and Riyadh; an Israeli strike kills
  Hamas security chief Abuelouf in Gaza.
- **Europe** — Ukraine hits two Samara refineries and an air base overnight;
  a Swedish Gripen was cleared to down a Russian missile over Poland on
  20 November, revealed today; Puigdemont says he will return to Spain on
  12 December.
- **Oceania** — Australia passes the Digital Duty of Care Bill; a bushfire
  emergency grips Tasmania's Flinders Island.
- **Sport** — Chess Game 2 is a 20-move draw, 1–1; in the Champions League,
  Lille stun Bayern 2–1, Liverpool cruise 3–0 at Club Brugge, PSG draw 2–2
  with Roma and Sporting draw 2–2 with Manchester United.

The page also carries a UTC timeline strip, a "day in numbers" strip
(9,500 lb of lead azide, KOSPI −6.16%, 31 killed in Cairo, US GDP 4.3%,
PCE 3.8%, Shenzhou liftoff 00:18 UTC, chess 1–1), a region bar, a dotted
world map ("Where it happened") with numbered pins, an "Also today" list of
20 more stories, and a red DATE CHECK box naming what was deliberately left
out because it happened on another day (the Riyadh tower strike of 24
November, the Huawei verdict of 24 November, the NATO AWACS deployment of
23 November, COP31 ending with no deal on 22 November, and more). Every
story is sourced; the sources are listed at the foot of the page. Press time
23:00 UTC.

## The bounty

Built for [make.fun](https://make.fun)'s
[`news-image-20261125`](https://make.fun/bounty/news-image-20261125) bounty:
sum up 25 November 2026's world news in one image. The prize pool is $100,
shared by the top 50 entries.

## How to run it

Node 22, standard library only — nothing to install. The program copies the
artwork into the output directory:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `entry.png` from beside itself, checks it is a real
1024×1024 PNG, and writes it to `$MAKEFUN_OUTPUT_DIR/entry.png` (or
`/output/entry.png` when the variable is not set). It refuses to run if the
artwork is missing, the wrong size, or not a PNG, and checks the copied
file's size and byte checksum match before reporting success.
