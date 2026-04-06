# GoDoStuffKIDS — Change Log
*Tracks changes in the main GoDoStuff app that may require action in the Kids app.*
*Updated whenever the main app ships a meaningful change to a city Kids covers.*

---

## How to use this file

When a change is logged, someone must decide:
- ✅ **Done** — change has been applied to Kids edition
- ⏳ **Review needed** — change needs to be assessed and applied
- ➡️ **Pass** — change is adult-specific, no Kids action needed
- 🔁 **New city** — Kids edition doesn't exist yet; add to queue

---

## 2026-04-05 / 2026-04-06 — Main app changes

### Nature walk entries added

| City | Kids edition? | Action |
|---|---|---|
| Amsterdam | ✅ Yes | ⏳ Review 6 new nature walk entries — likely all pass for Kids |
| Paris | ✅ Yes | ⏳ Review 6 new nature walk entries — likely all pass for Kids |
| London | ⏳ Queued | ➡️ No Kids edition yet — add to next Kids city queue |
| Vienna | ⏳ Queued | ➡️ No Kids edition yet |
| Prague | ⏳ Queued | ➡️ No Kids edition yet |
| Budapest | ⏳ Queued | ➡️ No Kids edition yet |
| Barcelona | ⏳ Queued | ➡️ No Kids edition yet |

**What to do:** Fetch the 6 nature walk entries added to Amsterdam and Paris from the main app, run them through the charter filter (they will pass — nature walks always pass), add quiz questions, add to Kids HTML files.

---

### Health notices added — Indian cities

| City | Kids edition? | Action |
|---|---|---|
| Delhi | ❌ No Kids edition | 🔁 When Delhi Kids is built, include "For Parents" health box |
| Mumbai | ❌ No Kids edition | 🔁 Same as Delhi |
| Chennai | ❌ No Kids edition | 🔁 Same as Chennai |

**What to do:** When Indian city Kids editions are built, reframe the health notice as a "For Parents:" box (not a traveller warning). Language: "Families find that bottled water is the standard here — it's what local families use too. Street food from busy stalls is generally fine. Ask your hotel or guesthouse what they recommend." Never alarmist.

---

### Conflict/war notices added

| City | Kids edition? | Action |
|---|---|---|
| Tel Aviv | ❌ No Kids edition | 🔁 When built: parents-only pre-visit note in city metadata; no war notice in entries |
| Kyiv | ❌ No Kids edition | 🔁 Same as Tel Aviv |

**What to do:** GoDoStuffKIDS never shows conflict notices inline. Instead, city metadata gets a `conflict_note_parents` field with a brief, calm note for parents: "This city is currently in an area of ongoing conflict. Please check current guidance before travelling. The entries below assume you are there and going out — the city's families continue their daily lives." Link to main GoDoStuff app for full conflict notice.

---

### Berlin cinematic enrichment (Apr 3)

| City | Kids edition? | Action |
|---|---|---|
| Berlin | ✅ Yes (103 entries) | ⏳ Review new entries — check if any pass Kids filter |

**What to do:** Fetch the ~25 new Berlin entries added in the cinematic enrichment. Review each against the Kids charter. Any that pass (likely history entries, viewpoints, hidden courtyards) should be added to the Berlin Kids edition with quiz questions.

---

### New cities enriched (no Kids edition yet)

The following cities were enriched in the main app but don't have Kids editions. They're added to the production queue in order of family travel demand:

**Priority queue:**
1. London (151 entries in main app — huge demand)
2. Vienna (135 entries)
3. Prague (140 entries)
4. Budapest (138 entries)
5. Barcelona (145 entries)
6. Tokyo (enriched Apr 3)
7. Naples (enriched Apr 3)
8. Lisbon
9. Rome
10. Copenhagen

---

## Template — future entries

```
## YYYY-MM-DD

### [Type of change]
| City | Kids edition? | Action |
|---|---|---|
| CityName | ✅/❌/⏳ | ⏳ Review / ➡️ Pass / 🔁 Queue |

**What to do:** [specific instruction]
```

---

*This log is maintained alongside the main GoDoStuff repo.*
*The goal: no change in the adult app that affects families goes unreviewed for the Kids edition.*
