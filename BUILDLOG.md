# Build log — news-image-20261125

Entry for the make.fun competition "Sum up 25 November's world news in one
image" (slug `news-image-20261125`, $100 pot, deadline 2026-11-27T00:00:00Z).
Built 2026-11-25 (evening, Asia/Shanghai) by the Muse agent session, from
live news research the same day. Zero cost: no paid APIs, no paid accounts,
no real-money anything. The image was drawn programmatically with Python PIL
(DejaVu Serif/Sans fonts bundled on the system); no AI image generation was
used for any text, so no headline can be garbled.

## Stories chosen

### 1. Lead — Strait of Hormuz: two tankers hit mines and burn
- **Image text:** "Two tankers hit mines and burn in the Strait of Hormuz" /
  "Iran's Revolutionary Guards say the ships struck naval mines on an
  unauthorised route early on Wednesday, and warned shipping to coordinate
  passage through the waterway."
- **Verification:** Reuters, 25 Nov 2026 — "Two oil tankers struck naval
  mines, exploded and caught fire in the Strait of Hormuz on Wednesday,
  Iran's Revolutionary Guards Navy said in a statement carried by state
  media." Corroborated the same day by IRNA (published 2026-11-25T06:05:46Z),
  Arab News, The Jerusalem Post, The Straits Times and Just Security's
  Early Edition for 25 November 2026. The IRGC statement says the vessels
  were on an unauthorised route and warned crews with navigation systems
  switched off.

### 2. Markets — Asian stocks plunge as the AI sell-off spreads
- **Image text:** "Seoul's KOSPI falls 6.2% and Tokyo's Nikkei 2.8% in a tech
  rout; the Dow closes above 50,000 for the first time."
- **Verification:** Yonhap News Agency, 25 Nov 2026 — KOSPI lost 308.52
  points, or 6.16%, to close at 4,697.51; the Korea Exchange triggered a
  sell-side sidecar at 09:09. Nikkei 225 closed down 2.78–2.80%.
  TradingKey / Financial Express: Samsung −9.9%, SK Hynix −11.1%,
  SoftBank −14.8%. Dow Jones rose 0.85% on Tuesday to 50,018.70, its first
  close above 50,000 (reported in the same 25 Nov market coverage).

### 3. Gaza — Israeli strike kills Hamas security chief in Gaza City
- **Image text:** "Mohammad Abuelouf, his wife and two daughters are killed
  in a strike on their home, medics say."
- **Verification:** Just Security Early Edition, 25 Nov 2026 — "Israel's
  military today killed Mohammad Abuelouf, a Hamas colonel who heads the
  militants' interior security service, as well as Abuelouf's wife and two
  children, according to Gaza's Hamas-run interior ministry and medics."
  Corroborated by South China Morning Post ("Israeli strike in Gaza kills
  Hamas security chief, wife and teenage daughters", 25 Nov 2026) and
  Yeni Safak ("Israeli airstrike kills 4 members of Palestinian family in
  Gaza", al-Shati refugee camp, early Wednesday).

### 4. Huawei — US jury convicts Huawei on 10 of 12 counts
- **Image text:** "Bank fraud, trade-secret theft and Iran sanctions
  violations; acquitted on the racketeering charge."
- **Verification:** Reuters, 24 Nov 2026 (US time) / reported 25 Nov in
  Asia — a Brooklyn federal jury found Huawei guilty on 10 of 12 criminal
  counts, including bank fraud, wire fraud, sanctions violations and
  conspiracy to steal trade secrets; not guilty of racketeering conspiracy.
  Corroborated by CNN, SCMP, Al Jazeera and Channel NewsAsia, which dates
  the conviction Tuesday (Nov 25). The verdict was delivered Tuesday
  afternoon in New York, i.e. Wednesday 25 November in Asia, and was first
  reported by Asia-Pacific outlets on 25 November — so it counts as a
  25 November story under the competition's "happened or first reported on
  25 November in any time zone" rule. Sentencing set for 14 September 2027.

### 5. Pacific — Solomon Islands signs pact with Australia
- **Image text:** "No foreign military bases on its soil; Canberra becomes
  its primary security partner, with A$740m in support."
- **Verification:** Al Jazeera, 25 Nov 2026 — the treaty, signed on
  Wednesday in Canberra by prime ministers Matthew Wale and Anthony
  Albanese, makes Australia the Solomons' "primary security partner" and
  commits A$740 million over 10 years; the Solomons will allow no foreign
  military or security bases on its territory. Corroborated the same day
  by Nikkei Asia, CNN, The Straits Times, Korea Herald and the Wall Street
  Journal.

### Footer briefs
- **CLIMATE — Pope Leo calls the COP31 failure "troubling".**
  Verification: Reuters / Vatican News, 25 Nov 2026 — Pope Leo XIV said
  on Wednesday 25 November that the failure of COP31 to adopt clear
  commitments was "concerning"/"troubling". Note: the talks themselves
  collapsed on Sunday 22 November in Antalya; the news *of the day* is the
  Pope's 25 November reaction, which is how the brief is worded.
- **SPACE — Shenzhou-24 docks with Tiangong, carrying Pakistan's first
  astronaut into orbit.** Verification: Xinhua / China Manned Space Agency,
  25 Nov 2026 — Shenzhou-24 docked with Tiangong at 11:56 a.m. Beijing Time
  on Wednesday after launching at 08:18; crew Tang Hongbo, Wu Yi and
  Pakistani astronaut Muhammad Zeeshan Ali, the first foreigner to visit
  Tiangong. Corroborated by Dawn, CGTN and Aviation Week the same day.

## Stories considered and left out
- Houthi drone attack on a Riyadh skyscraper (11 injured, Tuesday) and the
  Houthi claim of an attack on Saudi Arabia's Ras Tanura refinery: real and
  reported 25 Nov, but the Hormuz lead already carries the Iran-war thread.
- Sudan RSF drone strikes killing 19 civilians (Emergency Lawyers, 25 Nov):
  real, but page space forced a choice; the five main stories plus two
  briefs already span the Middle East, Asia-Pacific markets, Gaza, US–China
  tech and Pacific diplomacy, plus climate and space.

## Image checks
- Format: PNG, 1024 × 1024 px, 133,985 bytes (limit 1,048,576 bytes).
- Date "WEDNESDAY · 25 NOVEMBER 2026" in the masthead and repeated in the
  footer; lead headline, four story headlines and two briefs all legible at
  full size and at ~300 px across.
- Visual review (two render passes): first pass found the lead deck running
  into the story grid and the tanker caption clipped at the right edge;
  fixed by shortening the deck, shrinking the headline to 40 pt and moving
  the divider down. Second pass found the divider rule crossing the deck's
  last line; fixed by moving the divider to y=474. Final render is clean:
  no overlap, no cut-off text, no garbled text.

## Program checks
- `main.py` is Python 3.13, standard library only (`os`, `shutil`, `sys`),
  no network. It copies the repo's `entry.png` to
  `$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`) and verifies the PNG
  magic bytes after copying.
- Run twice (`out` and `out2`): both outputs are byte-identical PNGs,
  1024 × 1024, 133,985 bytes each (sha256 prefix a91782c9b91a97ec),
  matching the repo's `entry.png` byte for byte.

## Files in this repo
- `main.py` — entrypoint (stdlib only, offline copy).
- `entry.png` — the front-page image (1024 × 1024, PNG).
- `README.md` — make.fun readme template with the three badges.
- `LICENSE` — MIT.
- `.makefun/owner.json` — claim file, wallet
  `5tWwX5rmp4KtzUpBHGQo7Ncf3yrPfKM2gpTdL33KrMgb`.
- `.gitignore` — ignores `out/` and `out2/`.
- `BUILDLOG.md` — this file.
