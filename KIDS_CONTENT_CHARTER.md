# GoDoStuffKIDS — Content Charter
*The rules that govern everything in the Kids app. Every entry, every city, every update.*
*Last updated: April 2026*

---

## THE ONE SENTENCE

**The child asks "can we go out again?" — not "can I use the app?"**

Every content decision is tested against this. If an entry makes the city feel like homework, cut it. If it makes the city feel like an adventure, keep it.

---

## WHAT THIS APP IS

A city guide for families with children. The child is the primary audience — the app speaks to them, not to their parents. The parent is the enabler. The child is the explorer.

This app is **not** a filtered version of GoDoStuff. It is a different product with different entries, different writing, and different priorities. Some content overlaps. A lot does not.

---

## THE PIPELINE RULE

Every entry in GoDoStuffKIDS either:
- **Came from the main GoDoStuff app** — passed through the filter below, then enriched with Kids-specific fields (quiz, age range, honesty tags)
- **Was written fresh for Kids** — playgrounds, children's museums, farms, nature trails, puppet theatres, hands-on workshops that the adult app would never cover

A city's Kids edition should feel like it was written *for families*, not like the adult guide had its edges sanded off.

---

## THE FILTER — WHAT NEVER GOES IN

These are automatic disqualifications. No exceptions, no review required.

### Tags that are never imported from the main app
- `scary` — haunted houses, horror-themed anything, genuinely frightening spaces
- `abandoned` — derelict buildings, urban exploration, sites with real physical risk
- `romantic_water` — sunset boat trips, romantic lagoons (the framing is wrong for families)

### Content that is never written fresh for Kids
- Nightlife, bars, clubs, cocktail venues — even if "family-friendly until 10pm"
- Red-light districts or adult entertainment areas — even in a historical framing
- Extreme sports with genuine injury risk: cliff jumping, base jumping, free climbing
- Conflict zones or cities under active bombardment — no entry, no notice
- Any entry that mentions alcohol as a feature (wine regions, brewery tours, etc.)
- Gambling venues

### War and conflict notices
- GoDoStuff adult app may have war notices for Tel Aviv, Kyiv, etc.
- GoDoStuffKIDS **never** includes war or conflict notices in the city guide itself
- Instead: a **parents-only pre-visit note** in the city metadata (separate from entries) flagging that a city has an active situation, with a link to the GoDoStuff main app for full adult information
- The entries themselves assume the family is there and going out

---

## THE FILTER — WHAT ALWAYS PASSES

No review needed. These go straight through.

- `parks`, `lakes`, `swimming`, `day_trips`, `nature`, `sport`, `free_culture`
- Playgrounds — any kind
- Children's museums, science museums, natural history museums
- City farms, animal sanctuaries, petting zoos
- Puppet theatres, children's theatre, circus arts
- Hands-on workshops: baking, ceramics, printing, craft
- Gentle history: castles, old squares, market halls, old bridges
- Public transport adventures (train rides, tram rides, ferry crossings)
- Splash pads, fountains, rivers with paddling zones
- Viewpoints and hill climbs that are accessible and safe
- Street art and public sculpture
- Open-air markets (food markets, flower markets, craft markets)

---

## THE REVIEW LIST — HUMAN DECISION REQUIRED

These need a human to read the entry before it goes in.

| Tag / Content type | Why it needs review | Usually yes / usually no |
|---|---|---|
| `history_big` | Some history is great for kids; some needs adult context first | Castle sieges ✅ / detailed atrocity sites ❌ |
| `weird` | Weird street art = yes; weird adult bar = no | Unusual statues ✅ / taxidermy bar ❌ |
| `markets` | Most are great; some have adult product stalls | Food/flower ✅ / flea markets with adult content ❌ |
| `nerd` | Science = yes; heavily academic = maybe | Planetarium ✅ / archive reading room ❌ |
| `high_spots` | Most viewpoints are fine; some require dangerous access | Accessible tower ✅ / unguarded cliff edge ❌ |
| Health notices from main app | Reframe entirely — see below | See health section |
| Religious sites | Respectful visits are good; dress-code-heavy or very formal = review | Open cathedral ✅ / strict entry requirements for children ❌ |

---

## HEALTH NOTICES (India and similar cities)

The main GoDoStuff app has health/food/water notices for Indian cities (Delhi, Mumbai, Chennai) framed for adult travellers.

In GoDoStuffKIDS, health content is:
- **Placed as a "For Parents" box** — explicitly not addressed to the child
- **Framed practically**, not as a warning: "Here's what families find works well here"
- **Never alarmist** — the city is safe and wonderful; here's how to navigate it well
- **Includes local children** — "local kids play here safely every day"
- Bottled water is framed as "what everyone uses here, it's just how it works"

---

## WRITING RULES FOR KIDS ENTRIES

### Voice
- **Speak to the child, not the parent.** "You arrive to..." not "Parents will find..."
- **Present tense, active, immediate.** The adventure is happening now.
- **No warnings.** Practical information lives in the `t` (tip) field, written neutrally.
- **No fear language.** Not "be careful", not "watch out", not "dangerous if..."
- **Make it feel like a secret.** The child is finding something the city was hiding.

### Banned phrases (same as main app, plus Kids-specific)
- must-see, hidden gem, don't miss, perfect for, iconic, off the beaten path (inherited from main app)
- educational, learning opportunity, good for development (this is the death of fun)
- suitable for children, child-friendly, family-friendly (every entry IS for children — don't say it)
- be careful, watch out, adult supervision required (logistics go in `t`, never in `s` or `st`)

### The quiz rule
Every entry must have at least one quiz question. The question must be answerable **only by having been there** — not by googling. No trivia questions. Observation questions. "What colour was the door at the end of the courtyard?" not "What year was this building constructed?"

### Honesty tags
Every entry gets honesty tags. These are for the parent, brutally honest:
```
actually free | free unless your kid spots the kiosk | best before 11am
not worth a cross-town trip | amazing but short | bring spare socks
excellent with scooters | stroller hell | no shade | teen-safe vibes
meltdown exit nearby | toilet inside | crowded after 16:00 | fenced
open water — supervision required | bring own food | indoor escape nearby
```

---

## AGE FIELDS

Every entry has `age_min` and `age_max`. These are honest:
- age_min 2 = genuinely fine for toddlers
- age_min 6 = needs some ability to walk, follow instructions, engage
- age_min 10 = teenager territory — abstract thinking, sustained interest required
- age_max 14 = the upper Kids app range; adults can go but it's Kids content
- age_max 8 = genuinely loses its magic for older kids

The app filters by age. If you lie about age range, families show up and are disappointed. Don't lie.

---

## THE SYNC PROTOCOL WITH THE MAIN APP

GoDoStuff (adult) and GoDoStuffKIDS are separate products. They communicate through a structured protocol, not shared files.

### What triggers a Kids review
When the main app has changes to a city that Kids already covers, the following types of changes trigger a Kids review:

| Main app change | Kids action required |
|---|---|
| New entries added | Review each — does it pass the filter? Should Kids have it? |
| Entries edited (tone, content) | If the entry exists in Kids too, update it |
| Conflict/war notice added | Add parents-only pre-visit note to city metadata |
| Health notice added | Reframe as "For Parents" box |
| Nature walk entries added | High priority — almost always pass for Kids |
| Enrichment to 80+ entries | Check if Kids edition needs a top-up too |

### The CHANGE_LOG.md file
Every change to the main GoDoStuff app that affects a Kids city gets logged in:
`GODOSTUFF_KIDS_COWORK/CHANGE_LOG.md`

Format:
```
## 2026-04-06
- [MAIN APP] Amsterdam: +6 nature walk entries → KIDS REVIEW NEEDED
- [MAIN APP] Paris: +6 nature walk entries → KIDS REVIEW NEEDED
- [MAIN APP] Berlin: cinematic enrichment (+25 entries) → KIDS REVIEW IN PROGRESS
- [MAIN APP] Delhi: health notice added → KIDS: add "For Parents" box to city meta
- [MAIN APP] Tel Aviv: war notice → KIDS: add parents-only pre-visit note
- [MAIN APP] Kyiv: war notice → KIDS: add parents-only pre-visit note
```

### What does NOT sync automatically
- Tone-only changes in the adult app (different voice, doesn't carry over)
- Adult-specific entries (bars, nightlife, scary, abandoned)
- City enrichments for cities not yet in Kids

---

## CITIES IN KIDS — CURRENT STATUS

| City | Kids edition | Main app entries | Kids entries | Last synced |
|---|---|---|---|---|
| Berlin | ✅ Live (local) | 149+ | 103 | Apr 2026 |
| Amsterdam | ✅ Live (local) | 136 | TBC | Apr 2026 |
| Paris | ✅ Live (local) | 141 | TBC | Apr 2026 |
| Stockholm | ✅ Live (local) | TBC | TBC | Apr 2026 |
| London | ⏳ Queued | 151 | — | — |
| Vienna | ⏳ Queued | 135 | — | — |
| Prague | ⏳ Queued | 140 | — | — |

---

## GITHUB REPO

**Separate repo: `MariavHeland/godostuffkids`**

Reasons:
- Different product, different audience, different release cycle
- Kids app must be able to ship independently of the adult app
- Different content rules require separate review process
- Clean URL for app stores and sharing

Structure:
```
godostuffkids/
  index.html              ← city picker / home
  editions/
    berlin/index.html
    amsterdam/index.html
    paris/index.html
    stockholm/index.html
  manifest.json
  sw.js
  icon-192.png
  icon-512.png
```

---

*This document is the single source of truth for what goes into GoDoStuffKIDS.*
*When in doubt: would a 9-year-old be excited about this? Would their parent feel good about it? Both yes = it's in.*
