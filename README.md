# Oskar's Abu Dhabi Family Brief
A daily brief for a Swedish family moving to Abu Dhabi around May 2027: two parents, two children with a third on the way, a 3-year stay, a rented villa, two cars and a job in the city centre. It covers expat life, the family living environment, schools, housing, money, legislation and local news. It is a static GitHub Pages site (main, root) with no build step. The desert sand and teal theme lives in `style.css`. Sources are in SOURCES.md.

Cadence: Sunday to Friday at 06:30 Europe/Stockholm. Sunday covers Friday and Saturday, Monday covers everything since Sunday's edition, and other days cover since the previous edition (about 24h). Times are in Stockholm time (CET/CEST); UAE time is 3 hours ahead in winter and 2 in summer.

## Sections (class / chip)
| Class | Chip | Section | Covers |
|---|---|---|---|
| `safe` | Safety | Safety & regional security | Events touching the UAE; FCDO, US State Dept and Swedish UD/Regeringen advisory changes; embassy alerts; flights |
| `school` | Schools | Schools & childcare | ADEK rules, fees, admissions, new schools, inspections and ratings; British/IB/international and Nordic options; nurseries |
| `home` | Housing | Housing & neighbourhoods | Villa rents in Saadiyat, Yas, Al Reem, Khalifa City and Al Raha; rent cap, Tawtheeq, ADREC, market reports |
| `money` | Money | Money & cost of living | School fees, utilities, fuel and cars, groceries, banking, the AED peg; Swedish tax, ISK, exit and residency rules |
| `rules` | Rules | Rules, visas & legislation | Golden Visa and residency, ICP, labour and family law, licence conversion, health insurance |
| `health` | Health | Health & family | Hospitals, maternity, paediatrics, vaccinations, DoH rules |
| `life` | Life | Local life & weekends | Events, openings, weather, transport (Etihad Rail, roads), public holidays |
| `acc` | X | From the accounts we follow | Notable posts from SOURCES.md handles |
| `new` | New | New potentials (Sundays) | Verified sources to consider adding |

## Bilingual rule (English and Swedish side by side)
From 2026-10-29 every brief is bilingual. English sits in the left column (`.en`) and Swedish in the right column (`.sv`, `lang="sv"`), each pair wrapped in a `.bi` grid; `.lab` adds the small EN / SV labels. Below 760px the columns stack, English above Swedish. This applies to the headline and date, each hero card, each section title and description, each bullet, and the notes (gaps) block. Pages use `<body class="bil">` and `style.css?v=2`.
- The Swedish is a faithful, natural and idiomatic translation of the English: same facts, same caveats and flags (translate the flag text, e.g. "single source" = "en enda källa"), nothing added or dropped.
- Links are identical in both columns, in the same order.
- Use official Swedish terms: UD, avrådan, Regeringen, Skatteverket, ISK, uppehållstillstånd. Keep UAE proper names (ADEK, ADREC, Tawtheeq, Golden Visa, Emirates ID) as they are. Swedish dates and times: "torsdag 29 oktober", "kl. 06.30", "14,9 °C", "160 000 AED".
- Section chips read in Swedish: Säkerhet, Skolor, Boende, Pengar, Regler, Hälsa, Livet, X, Nytt; hero chips read "Safety · Säkerhet".
- No em-dashes or en-dashes in either language; write "33 till 37".
- Editions before 2026-10-29 stay English only.

## Add a brief
1. Copy `template.html` to `briefs/YYYY-MM-DD.html` and fill `{{DATE}}`, `{{DATE_LONG_EN}}` / `{{DATE_LONG_SV}}` (add " · Weekend edition" / " · Helgutgåva" on Sundays) and `{{HEADLINE_EN}}` / `{{HEADLINE_SV}}` (optionally wrap the same key phrase in `<mark>` in both).
2. Hero: 4 story cards (copy the S1 article), with the class taken from the table above, and both `_EN` and `_SV` fields filled.
3. Fill each `{{..._ITEMS}}` with 1-4 `<li class="bi"><div class="en">English</div><div class="sv" lang="sv">Svenska</div></li>` bullets. Each bullet is one or two sentences with the source link inline, and says why it matters to the family when that is not obvious. Mark weak items with `<span class="flag">single source</span>` (Swedish: `en enda källa`) in both columns. For an empty section use `<li class="bi empty"><div class="en">Quiet.</div><div class="sv" lang="sv">Lugnt.</div></li>`. Items older than the window must carry their date.
4. Safety tone: factual and calm. Say clearly what did *not* happen, for example "no change to the advisory level" or "no attack on UAE territory reported". Always state the current US level and whether the UK FCDO and Swedish UD pages changed.
5. `{{NOTES_EN}}` / `{{NOTES_SV}}`: the window, paywalled or failed sources, and unconfirmed items.
6. In `index.html`, add under `<!-- ARCHIVE: newest first -->`:
   `<a class="bcard wide" href="briefs/YYYY-MM-DD.html"><div class="d">DATE_LONG_EN · DATE_LONG_SV</div><div class="h bi lab"><div class="en">HEADLINE_EN</div><div class="sv" lang="sv">HEADLINE_SV</div></div></a>`
   Only the newest card is `wide`; when adding a new one, remove `wide` from the previous card (it can stay bilingual).
7. No em-dashes. Never invent facts. Flag single-source or unconfirmed items. Prefer primary sources (ADEK, ADREC, ADRO/ICP, DoH, embassies) over visa or property blogs. Then `git commit`, `git push` to main and check that the page returns 200.
