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

## Add a brief
1. Copy `template.html` to `briefs/YYYY-MM-DD.html` and fill `{{DATE}}`, `{{DATE_LONG}}` (add " · Weekend edition" on Sundays) and `{{HEADLINE}}` (optionally wrap one key phrase in `<mark>`).
2. Hero: 4 story cards (copy the S1 article), with the class taken from the table above.
3. Fill each `{{..._ITEMS}}` with 1-4 `<li>` bullets. Each bullet is one or two sentences with the source link inline, and says why it matters to the family when that is not obvious. Mark weak items with `<span class="flag">single source</span>`. For an empty section use `<li class="empty">Quiet.</li>`. Items older than the window must carry their date.
4. Safety tone: factual and calm. Say clearly what did *not* happen, for example "no change to the advisory level" or "no attack on UAE territory reported". Always state the current US level and whether the UK FCDO and Swedish UD pages changed.
5. `{{NOTES}}`: the window, paywalled or failed sources, and unconfirmed items.
6. In `index.html`, add under `<!-- ARCHIVE: newest first -->`:
   `<a class="bcard" href="briefs/YYYY-MM-DD.html"><div class="d">DATE_LONG</div><div class="h">HEADLINE</div></a>`
7. No em-dashes. Never invent facts. Flag single-source or unconfirmed items. Prefer primary sources (ADEK, ADREC, ADRO/ICP, DoH, embassies) over visa or property blogs. Then `git commit`, `git push` to main and check that the page returns 200.
