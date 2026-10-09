# Pronunciation Guide for Suno Lyrics

Suno's text-to-speech engine can mispronounce words, especially homographs (same spelling, different pronunciation) and technical terms. This guide helps identify problem words and provides solutions.

> **Related skill**: `/bitwize-music:pronunciation-specialist` (automated scanning for pronunciation risks)
> **Related docs**: [best-practices.md](best-practices.md)

## Why This Matters

Suno reads lyrics literally. It doesn't understand context the way humans do. When it sees "live," it picks one pronunciation — and it might be wrong for your meaning.

**Note**: Suno's context sensitivity for pronunciation is limited, so the rule stands: **never trust context for homographs**. Context sensitivity alone is not reliable enough to skip phonetic spelling.

**IPA Note**: IPA (International Phonetic Alphabet) is **not natively supported** by Suno despite community requests. Use the phonetic spelling approaches documented below instead.

**Example**: "LiveJournal confessions" was sung as "LIV-journal" (like a live performance) instead of "LYVE-journal" (like alive).

## Homographs Reference

Words spelled the same but pronounced differently depending on meaning.

### High-Risk Homographs

| Word | Pronunciation A | Pronunciation B | Example Context |
|------|-----------------|-----------------|-----------------|
| **live** | /lɪv/ (LIV) - live performance, live show | /laɪv/ (LYVE) - alive, living, to reside | See detailed "live" section below |
| **read** | /riːd/ (REED) - present tense | /rɛd/ (RED) - past tense | "I read it yesterday" = RED |
| **lead** | /liːd/ (LEED) - guide, metal band | /lɛd/ (LED) - the metal | "Lead pipes" = LED |
| **wind** | /wɪnd/ (WIND) - breeze | /waɪnd/ (WYND) - turn, coil | "Wind the clock" = WYND |
| **close** | /kloʊs/ (KLOHS) - near | /kloʊz/ (KLOHZ) - shut | "Close the door" = KLOHZ |
| **tear** | /tɪr/ (TEER) - from crying | /tɛr/ (TAIR) - rip | "Tear the page" = TAIR |
| **bow** | /boʊ/ (BOH) - ribbon, weapon | /baʊ/ (BOW) - bend, ship front | "Take a bow" = BOW |
| **bass** | /beɪs/ (BAYSS) - instrument, low freq | /bæs/ (BASS) - the fish | Usually BAYSS in music |
| **row** | /roʊ/ (ROH) - line, propel boat | /raʊ/ (ROW) - argument | "Row of seats" = ROH |
| **sow** | /soʊ/ (SOH) - plant seeds | /saʊ/ (SOW) - female pig | "Sow the seeds" = SOH |
| **wound** | /wuːnd/ (WOOND) - injury | /waʊnd/ (WOWND) - coiled | "Wound around" = WOWND |
| **minute** | /ˈmɪnɪt/ (MIN-it) - 60 seconds | /maɪˈnjuːt/ (my-NOOT) - tiny | "Minute details" = my-NOOT |
| **resume** | /rɪˈzuːm/ (ri-ZOOM) - continue | /ˈrɛzjʊmeɪ/ (REZ-oo-may) - CV | Usually ri-ZOOM |
| **object** | /ˈɒbdʒɪkt/ (OB-jekt) - thing | /əbˈdʒɛkt/ (ob-JEKT) - protest | "I object" = ob-JEKT |
| **project** | /ˈprɒdʒɛkt/ (PROJ-ekt) - plan | /prəˈdʒɛkt/ (pro-JEKT) - throw | "Project your voice" = pro-JEKT |
| **record** | /ˈrɛkərd/ (REK-ord) - noun | /rɪˈkɔːrd/ (ri-KORD) - verb | "Record a song" = ri-KORD |
| **present** | /ˈprɛzənt/ (PREZ-ent) - gift, here | /prɪˈzɛnt/ (pri-ZENT) - give | "Present the award" = pri-ZENT |
| **content** | /ˈkɒntɛnt/ (KON-tent) - stuff | /kənˈtɛnt/ (kon-TENT) - satisfied | "I'm content" = kon-TENT |
| **desert** | /ˈdɛzərt/ (DEZ-ert) - sandy place | /dɪˈzɜːrt/ (di-ZURT) - abandon | "Desert the cause" = di-ZURT |
| **refuse** | /ˈrɛfjuːs/ (REF-yoos) - garbage | /rɪˈfjuːz/ (ri-FYOOZ) - decline | "I refuse" = ri-FYOOZ |

### Detailed: "live" Pronunciation Fixes

The word "live" is one of the most common pronunciation problems in Suno. **Always clarify which meaning is intended.**

#### LYVE (rhymes with "five") - alive, living, to reside

| Intended | Problem | Fix Options |
|----------|---------|-------------|
| "live your life" | May say LIV | Use "lyve your life" or rewrite to "living your life" |
| "live and breathe" | May say LIV | Use "lyve and breathe" or "alive and breathing" |
| "I live here" | May say LIV | Use "I lyve here" or "I'm living here" or "I reside here" |
| "LiveJournal" | May say LIV-journal | Use "Life-journal" or "Lyve-journal" |
| "live wire" | May say LIV wire | Use "lyve wire" |
| "alive" | Usually fine | No fix needed |
| "living" | Usually fine | No fix needed |

#### LIV (rhymes with "give") - live performance, live show, broadcasting

| Intended | Problem | Fix Options |
|----------|---------|-------------|
| "live performance" | May say LYVE | Use "liv performance" or rewrite to "performing live" |
| "live show" | May say LYVE | Use "liv show" or "concert" |
| "live broadcast" | May say LYVE | Use "liv broadcast" or "broadcasting now" |
| "live audience" | May say LYVE | Use "liv audience" or "studio audience" |
| "going live" | May say LYVE | Use "going liv" or "on air now" |
| "live stream" | May say LYVE | Use "liv stream" or "streaming now" |

#### Quick Decision Guide

Ask yourself: **Does it rhyme with "five" or "give"?**

- "I want to **live** my dreams" → LYVE (rhymes with five) → use "lyve" or "living"
- "We're going **live** on air" → LIV (rhymes with give) → use "liv" or rewrite

### Medium-Risk Homographs

| Word | Pronunciations | Notes |
|------|---------------|-------|
| **alternate** | ALL-ter-nit (adj) / ALL-ter-nayt (verb) | Context usually clear |
| **attribute** | AT-trib-yoot (noun) / a-TRIB-yoot (verb) | Context usually clear |
| **combine** | KOM-byne (noun, farm) / kom-BYNE (verb) | Rare noun usage |
| **complex** | KOM-pleks (noun) / kom-PLEKS (adj) | Usually adjective |
| **conduct** | KON-dukt (noun) / kon-DUKT (verb) | Context usually clear |
| **conflict** | KON-flikt (noun) / kon-FLIKT (verb) | Usually noun |
| **console** | KON-sole (noun) / kon-SOLE (verb) | Tech context = noun |
| **contract** | KON-trakt (noun) / kon-TRAKT (verb) | Context usually clear |
| **contrast** | KON-trast (noun) / kon-TRAST (verb) | Context usually clear |
| **convert** | KON-vert (noun) / kon-VERT (verb) | Usually verb |
| **convict** | KON-vikt (noun) / kon-VIKT (verb) | Context usually clear |
| **decrease** | DEE-krees (noun) / dee-KREES (verb) | Context usually clear |
| **digest** | DY-jest (noun) / dy-JEST (verb) | Context usually clear |
| **discount** | DIS-count (noun) / dis-COUNT (verb) | Context usually clear |
| **exploit** | EKS-ploit (noun) / eks-PLOIT (verb) | Tech context = noun |
| **extract** | EKS-trakt (noun) / eks-TRAKT (verb) | Context usually clear |
| **impact** | IM-pakt (noun) / im-PAKT (verb) | Usually noun |
| **import** | IM-port (noun) / im-PORT (verb) | Context usually clear |
| **incline** | IN-klyne (noun) / in-KLYNE (verb) | Context usually clear |
| **increase** | IN-krees (noun) / in-KREES (verb) | Context usually clear |
| **insert** | IN-sert (noun) / in-SERT (verb) | Context usually clear |
| **insult** | IN-sult (noun) / in-SULT (verb) | Context usually clear |
| **invalid** | IN-va-lid (adj, not valid) / in-VA-lid (noun, sick person) | Rare noun |
| **misprint** | MIS-print (noun) / mis-PRINT (verb) | Rare word |
| **moderate** | MOD-er-it (adj) / MOD-er-ayt (verb) | Context usually clear |
| **perfect** | PER-fekt (adj) / per-FEKT (verb) | "Perfect the art" = verb |
| **permit** | PER-mit (noun) / per-MIT (verb) | Context usually clear |
| **pervert** | PER-vert (noun) / per-VERT (verb) | Usually noun |
| **produce** | PROD-oos (noun) / pro-DOOS (verb) | "Fresh produce" = noun |
| **progress** | PROG-ress (noun) / pro-GRESS (verb) | Context usually clear |
| **protest** | PRO-test (noun) / pro-TEST (verb) | Context usually clear |
| **rebel** | REB-el (noun) / ri-BEL (verb) | "I rebel" = verb |
| **recount** | REE-count (noun) / ree-COUNT (verb) | Context usually clear |
| **refund** | REE-fund (noun) / ree-FUND (verb) | Context usually clear |
| **reject** | REE-jekt (noun) / ri-JEKT (verb) | Usually verb |
| **relay** | REE-lay (noun) / ree-LAY (verb) | Context usually clear |
| **segment** | SEG-ment (noun) / seg-MENT (verb) | Usually noun |
| **separate** | SEP-er-it (adj) / SEP-er-ayt (verb) | Context usually clear |
| **subject** | SUB-jekt (noun) / sub-JEKT (verb) | "Subject to" = verb |
| **survey** | SUR-vay (noun) / sur-VAY (verb) | Context usually clear |
| **suspect** | SUS-pekt (noun) / sus-PEKT (verb) | Context usually clear |
| **torment** | TOR-ment (noun) / tor-MENT (verb) | Context usually clear |
| **transfer** | TRANS-fer (noun) / trans-FER (verb) | Context usually clear |
| **transport** | TRANS-port (noun) / trans-PORT (verb) | Context usually clear |
| **upset** | UP-set (noun/adj) / up-SET (verb) | Usually adjective |

## Tech Terms & Brand Names

### Compound Brand Names

| Term | Correct | Wrong | Fix |
|------|---------|-------|-----|
| LiveJournal | LYVE-journal | LIV-journal | Write "Life-journal" or rewrite |
| YouTube | YOU-toob | yoo-TOOB | Usually fine, but watch for emphasis |
| GitHub | GIT-hub | GITH-ub | Usually fine |
| MySpace | MY-space | MICE-pace | Usually fine |
| GeoCities | JEE-oh-cities | GEO-cities | Usually fine |
| CompuServe | kom-pyu-SERV | Usually fine | - |
| SoundCloud | SOUND-cloud | Usually fine | - |
| Usenet | YOOZ-net | YOOS-net | Either acceptable |

### Acronyms & Initialisms

#### Suno-Specific Spelling for Correct Pronunciation

Some terms need special spelling in lyrics to get Suno to pronounce them correctly:

| Term | Correct Pronunciation | Write As | Notes |
|------|----------------------|----------|-------|
| GNU | "guh-NEW" (hard G) | **guh-new** | Without this, Suno may say "G-N-U" or "new" |
| Debian | "DEB-ee-un" | **Deb-Ian** | Hyphen ensures three syllables |

#### Letter-by-Letter Acronyms

Use periods between letters to force Suno to spell them out:
- **S.L.S.** not "SLS"
- **L.K.M.L.** not "LKML"
- **B.D.F.L.** not "BDFL"
- **D.F.S.G.** not "DFSG"
- **A.P.I.** not "API"

Without periods, Suno may try to pronounce letter-acronyms as words.

#### Standard Acronym Pronunciations

| Term | Pronunciation | Notes |
|------|--------------|-------|
| SQL | "sequel" or "S-Q-L" | Both used, "sequel" more common |
| GUI | "gooey" | Not "G-U-I" |
| API | "A-P-I" | Spell it out |
| URL | "U-R-L" or "earl" | Spell out preferred |
| GIF | "jif" or "gif" | Contested - avoid if possible |
| IEEE | "eye-triple-E" | Not "I-E-E-E" |
| BIOS | "BY-ose" | Not "B-I-O-S" |
| ASCII | "ASK-ee" | Not "A-S-C-I-I" |
| SCSI | "scuzzy" | Not "S-C-S-I" |
| WYSIWYG | "WIZ-ee-wig" | The what-you-see acronym |
| FAQ | "fak" or "F-A-Q" | Both used |
| PNG | "ping" or "P-N-G" | Both used |
| JPEG | "JAY-peg" | Not "J-P-E-G" |
| MIDI | "MID-ee" | Not "M-I-D-I" |
| WiFi | "WY-fy" | Not "wiff-ee" |
| SaaS | "sass" | Not "S-A-A-S" |
| LED | "L-E-D" | Spell it out |
| RAM | "ram" | Like the animal |
| ROM | "rom" | Rhymes with Tom |
| DOS | "doss" | Not "D-O-S" |
| LAN | "lan" | Rhymes with pan |
| WAN | "wan" | Rhymes with John |

### Tech Words

| Term | Correct | Common Mistake |
|------|---------|---------------|
| Linux | LIN-ucks | LINE-ucks |
| data | DAY-ta or DAT-a | Both acceptable |
| cache | "cash" | "catch" or "cash-ay" |
| daemon | DEE-mon | DAY-mon |
| byte | "bite" | - |
| pixel | PIK-sel | - |
| router | ROW-ter (US) or ROOT-er (UK) | Context-dependent |
| admin | AD-min | Not "add-MEEN" |
| sudo | "SOO-doo" or "SOO-doh" | Not "pseudo" |
| root | "root" | - |
| kernel | KER-nel | - |
| chmod | "ch-mod" or "change-mod" | - |
| grep | "grep" (rhymes with step) | - |
| wget | "w-get" or "double-you-get" | - |
| regex | "REJ-eks" | Not "REE-jeks" |
| tuple | "TUP-el" or "TOO-pel" | Both used |

## Fixes & Workarounds

### Option 1: Rewrite (Preferred)

Find alternative phrasing that avoids the problem word entirely.

**Before**: "LiveJournal confessions in abandoned rooms"
**After**: "Old blog confessions in abandoned rooms"

**Before**: "I read your message yesterday"
**After**: "I saw your message yesterday"

### Option 2: Phonetic Spelling

Write the word how it sounds. Looks weird in lyrics but works.

| Original | Phonetic | Use When |
|----------|----------|----------|
| LiveJournal | Life-journal | Brand pronunciation critical |
| read (past) | red | Past tense ambiguous |
| lead (metal) | led | Metal meaning needed |
| wound (coil) | wownd | Coil meaning needed |
| live (alive) | lyve | Alive/living meaning (rhymes with "five") |
| live (performance) | liv | Live show/broadcast meaning (rhymes with "give") |

### Option 3: Hyphenation

Break syllables to guide pronunciation. Can help with sustained notes too.

| Original | Hyphenated | Effect |
|----------|-----------|--------|
| live (alive) | li-ive | Forces long 'i' |
| read (present) | ree-ead | Forces long 'e' |
| wind (coil) | wi-ind | Forces long 'i' |

### Option 4: Context Padding

Add words that make the pronunciation obvious.

**Before**: "Live broadcast from the scene"
**After**: "Broadcasting live from the scene" (verb form clearer)

**Before**: "The lead singer"
**After**: "Leading the band" (verb form avoids ambiguity)

### Option 5: Accept It

Sometimes the mispronunciation isn't jarring enough to matter, or there's no good fix. Document the risk and move on.

## Pronunciation Table Enforcement Workflow

The Pronunciation Notes table in each track file is a **mandatory checklist**, not passive documentation. Every entry MUST be applied as phonetic spelling in the Suno Lyrics Box.

### Process

1. **Before finalizing any track**: Read the Pronunciation Notes table top to bottom
2. **For each entry**: Search the Suno Lyrics Box for the standard spelling
3. **Replace** with the phonetic version from the table
4. **Verify** every occurrence is fixed — check all verses, choruses, bridges, and outros
5. **Common failure**: Word added to table but never applied to lyrics, or phonetic in one verse but missed in chorus/bridge

### Verification Format

After applying all phonetics, document verification:

```markdown
| Word | Standard | Phonetic | Applied? |
|------|----------|----------|----------|
| Ramos | Ramos | Rah-mohs | ✓ All 4 occurrences |
| live | live | lyve | ✓ V1, V2, Chorus |
| FBI | FBI | F-B-I | ✓ Bridge |
```

### Rules

- The table is the source of truth — if it says phonetic, the Suno lyrics MUST use phonetic
- Streaming/distributor lyrics always keep standard English spelling
- When adding a new word to the table, immediately apply it to all Suno lyrics
- Run this check as the final step before generation, after all other edits are complete

## Numbers

Always **spell out numbers** in Suno lyrics — Suno handles written-out numbers more reliably than digits.

| Write | Not |
|-------|-----|
| twenty-one | 21 |
| nineteen eighty-four | 1984 |
| three hundred | 300 |

**Exception**: Year abbreviations like `'93` work well and avoid the "ninety-three" producer tag filter issue.

---

## Multilingual Tracks

For songs with lyrics in multiple languages:

- **Use one language per section** — mixing languages within a section causes pronunciation drift
- Add `all lyrics in [language], no English` to the style prompt for non-English sections to prevent the model reverting to English
- Section isolation remains the most reliable approach for multilingual tracks

**Example**:
```
[Verse 1 - Spanish]
Spanish lyrics here...

[Chorus - English]
English chorus here...
```

Style prompt: Include both language indicators: "bilingual, Spanish verse, English chorus"

---

## German Pronunciation

Suno interprets German vowels using English phonetic rules, which causes specific mispronunciations. These fixes apply to **all German-language lyrics**, regardless of genre.

### Short vs Long Vowels

Suno treats single German vowels as short English vowels. To force the correct long German pronunciation, **double the vowel**.

| German Word | Suno Reads As | Fix | Why |
|-------------|---------------|-----|-----|
| juchhe | "juch-heh" (short e) | **juchee** | Double-e forces long "ee" sound |
| Schnee | "schneh" (short e) | **Schnee** (usually OK) | Double-e already present |
| See | "seh" (short e) | **See** (usually OK) | Double-e already present |

**Rule of thumb**: If a German word ends in a single vowel that should be long, double it for Suno. Test by generating — if the vowel sounds clipped, double it.

### German Umlauts

Suno handles umlauts inconsistently. Test first, fix if needed.

| Character | Suno Behavior | Fix If Wrong |
|-----------|--------------|--------------|
| ä | Sometimes reads as "a" | Use "ae" |
| ö | Sometimes reads as "o" | Use "oe" |
| ü | Sometimes reads as "u" | Use "ue" |
| ß | Usually reads as "ss" | Usually OK |

### German Interjections

Common German exclamations that Suno may mispronounce:

| Word | Expected | Suno Risk | Fix |
|------|----------|-----------|-----|
| juchhe | "juch-HEE" | Short clipped "heh" | **juchee** |
| juhu | "yoo-HOO" | May stress wrong syllable | Usually OK |
| hurra | "hoo-RAH" | Usually OK | — |
| ach | "ahh" (guttural) | May say "atch" | Usually OK |
| oho | "oh-HOH" | Usually OK | — |

---

## Czech Pronunciation

These fixes apply to **all Czech-language lyrics**, regardless of genre. Czech spelling is phonemic: each letter maps almost one-to-one to a sound. So once Suno recognises a line as Czech, most native words should come out right without help. The risks are concentrated in a few letters, in words that look English, in slang, in numbers, and in stress. Test first, fix if needed.

**Evidence status.** We found no first-hand, Czech-specific pronunciation test on v4.5, v5, v5.5 or v6. Every Czech report comes from the v3–v4.5 era or carries no date, and all pre-v6 models were retired on 2026-09-09. Treat this section as a starting point and re-test on v6. Each claim carries one of these labels:

| Label | Meaning |
|-------|---------|
| **verified** | We read the source text or the Suno metadata ourselves. This confirms what the source says, not that the plugin tested the claim on Czech. |
| **reported** | A community or vendor report. Nobody on this project tested it. |
| **untested** | Our reasoning from Czech phonology or from another language. No Suno test exists. |

### What's Known

| Claim | Status | Source |
|-------|--------|--------|
| Suno sings Czech "decently" (*slušně*), but pronunciation sometimes slips on longer or more complex lyrics | reported | aifirst.cz (undated), pisnickynakrizovatce, Lupa.cz (Mar 2024, v3, from social-media examples rather than its own test) |
| Czech is not on any published list of best-supported languages, and less-represented languages may get an accent or imprecise pronunciation. Suno publishes no official language list. | reported | d3arts.cz (v5.5 guide, Jun 2026), aifirst.cz |
| The model reads word by word and guesses each word. Czech words that look English get English pronunciation ("statisticky"), and some words come out with a foreign, "Balkan" accent ("dokázáno"). | reported | Živě.cz (v3 era; read only through a search snippet, because the page was blocked) |
| The song drifts into another language partway through, mainly on v1/v2 | reported | pisnickynakrizovatce |
| English words and foreign names inside Czech lyrics should be rewritten the way they are pronounced | reported | pisnickynakrizovatce, VeŠkole.cz (Oct 2024). Neither gives examples. |
| "Use native script first … test transliteration only when the native spelling fails" | verified (general advice, not Czech-specific) | Jack Righteous multilingual guide |
| Long lines with too many syllables cause "rushed delivery, swallowed consonants and strange stress". The fix is to split the line. | verified (general advice, not Czech-specific) | Jack Righteous v5.5 fix guide |
| Some Czech songs on v4.5 (one playlist checked, two creators) write the language into the style prompt ("Lyrics in Czech", "intimate male Czech vocal lead"). The v3.5 Czech/Slovak playlist checked used no language tag at all. | verified as practice only, not as effective | suno.com song metadata |
| Suno's v6 announcement makes no claim about languages other than English, diction or pronunciation. One report says non-English output got worse on v6 (one scripted video, no example). Nothing is Czech-specific. | verified (announcement text); the degradation report is reported and not adopted | [Suno — Introducing v6](https://suno.com/blog/introducing-v6) (9 Sep 2026); [CHANGELOG.md](CHANGELOG.md) |
| How Suno handles individual letters (ř, ě, ů, ch, c) | untested: no source documents it | — |

### Keep Diacritics

**Never strip háčky, čárky or the kroužek** (ˇ ´ ˚). Status: **untested**, but well supported. No source has tested stripping diacritics in any language. However:
- Czech diacritics change sounds and words.
- Stripped Czech often looks like English, and Suno predicts pronunciation from spelling, with no dictionary or IPA (HookGenius, vendor claim).
- A Polish guide gives the same advice for Polish *ogonki*, though its author says outright that he ran no listening test (promptowy.com, 2026-09-12).

| With Diacritics | Stripped | What Goes Wrong |
|-----------------|----------|-----------------|
| být (to be) | byt | A different word ("flat") |
| řada (row) | rada | A different word ("advice") |
| šít (to sew) | sit | Reads as the English word "sit" |
| pás (belt) | pas | A different word ("passport") |
| čas (time) | cas | Loses the "č" and looks foreign |
| česky (in Czech) | cesky | Looks English, so the c may come out as "s" or "k" |

**Rule of thumb**:
- Keep standard Czech spelling.
- Respell **one word at a time**, and only after you have heard that word fail.
- Use the same respelling everywhere the word appears.
- Never respell with a global find-and-replace (promptowy, reported).
- Record every respelling in the track's Pronunciation Notes table. Streaming and distributor lyrics keep the normal Czech spelling.

**Do not port the German or English-style fixes** (untested reasoning):
- **Doubled vowels** (juchee): Czech already marks length with á é í ý ó ú ů, so "aa" risks being sung as two syllables.
- **Umlaut → ae/oe**: Czech has no equivalent, and spelling ř as "rz" is Polish orthography that may pull the line toward Polish pronunciation.
- **English-style respelling of native words** (Ho-zay): Czech spelling is already phonetic, and an English respelling invites English letter rules.

### Style Prompt: Language Lock

Write the Style Box in **English** and only the lyrics in Czech. Status: **reported** (tomoviny.cz, HookGenius and sunomarket all agree).

Name the language with positive descriptors. Sunomarket's warning, "Do not assume Suno will infer the language", is **reported** and was written for other languages. The exact wording below is **untested** for Czech.

```
Style: czech rap, czech lyrics, all lyrics in Czech, male Czech rap vocal,
native Czech diction, clear articulation, dark trap beat, 808s, 140 BPM half-time
Exclude Styles: English accent
```

- **Don't count on an inline "no English".** v6 ignores exclusions written into the prompt (see [Negative Prompting](best-practices.md#negative-prompting)). The "all lyrics in [language], no English" line in § Multilingual Tracks above predates that rule, and we found no current source for it.
  - Put the exclusion in the **Exclude Styles** field instead, as a bare element: `English accent`. This is **reported** by sunomarket and untested for Czech.
  - If takes still drift toward English, add `English lyrics` as well. This is from sunomarket's example Exclude list (reported) and untested for Czech.
- **Variety Off.** Above Off, Suno rewrites the Style Box ([best-practices.md](best-practices.md)). That rewrite could dilute the Czech descriptors (untested).
- **No artist names.** Describe the sound instead ("dark Czech trap, melodic auto-tuned hook, 808s"); see [artist-blocklist.md](artist-blocklist.md). Whether Suno filters Czech rappers' names is untested.
- **Section labels** like `[Verse 1 - Czech]` are "an experiment, not a guarantee" (Jack Righteous, verified text). Use them if you like, but don't rely on them.

### Risky Letters and Clusters

No source documents how Suno handles individual Czech letters, so **every row in this table is untested**. The risk predictions follow from Suno reading pronunciation off spelling: the danger is greatest in words that also look English or international, and on held notes. Test first, fix if needed.

| Letter / Pattern | Czech Sound | Suno Risk (untested) | Fix If Wrong |
|------------------|-------------|----------------------|--------------|
| ř (řeka, moře, tři, přes, dřív) | One sound: a raised trilled r with ž-like friction (řeka, moře, dřív). After p/t/k and at the end of a word it is voiceless, closer to r + š (tři, přes, keř). | Flattened to plain r or ž, especially on a held note or at the end of a bar | Rewrite the line, or swap in a synonym, so ř is not on a held note or a bar end. Last resort, for that one word only, and only at the start of a word or after a vowel: "rž" (řeka → ržeka, moře → morže). After a consonant (dř, tř, př, kř, hř…), any r + consonant spelling makes the r syllabic and adds a syllable (dřív → držív reads dr-žív; tři → trži reads tr-ži), so there you must rewrite the line. Never use "rz", which is Polish spelling. |
| ě (věc, pět, děti, mě) | "je" after b/p/v; softens d/t/n (děti = ďeti); "mňe" after m. Note that mě and mně sound the same. | Read as a plain e, losing the j-glide or the softening | Usually OK. If the softening is lost after d/t/n, respell with the soft consonant: děti → ďeti, tělo → ťelo. |
| ů (dům, můj, půl) | A long u, the same sound as ú | Unfamiliar outside Czech, so it may be read short or wrong | Usually OK. If clipped, use ú, which is the same sound in Czech: dům → dúm. Never double it ("uu"). |
| ch (chci, prach, ticho, chata) | A voiceless "kh" made at the back of the mouth (velar [x]), as in Scottish "loch". Not the same as Czech h, which is voiced (hora). | English "tch" (or "k") in words that look English (chill, chaos, chata) | Native words are usually OK in a clearly Czech line. If one comes out as "tch", rewrite with a different word. For an English loan, spell its intended sound the Czech way (chill → čil). |
| c (cena, ulice, cíl) | "ts" | English "k" or "s" (cena → "sena") | Rewrite first. Last resort, for that one word: "ts" (cena → tsena). |
| č, š, ž | "ch", "sh", "zh" | Low, as long as the háček is kept | Never strip the háček. |
| j (já, jo, jsem) | English "y" | English "dj" in words that look English | Usually OK. jsem/jsi/jsou are spoken without the j; if the song is written in colloquial register, write sem/seš/sou (seš only as a full verb: seš borec; the past-tense auxiliary jsi becomes si or -s: byl si, kdes byl, never 'byl seš'). |
| Syllabic r/l (vlk, smrt, prst, Brno, Vltava) | r or l acts as the vowel: vlk = 1 syllable, Brno = 2, Vltava = 3 | An extra vowel gets inserted ("smert") or the syllable is swallowed, which breaks the syllable count | Hyphenate at the syllable break (Br-no, čtvr-tek, Vl-ta-va). Never write in a vowel. |
| Consonant clusters (čtvrtek, zmrzlina, scvrklý, vzpomínky) | All consonants pronounced, but voicing assimilates to the last consonant of the cluster: vzpomínky = 'fspomínky', kdo = 'gdo', tužka = 'tuška'. | Turns to mush at rap speed. This is reported for Russian and Polish clusters (sunomarket) but not tested on Czech. | Rewrite fast or triplet passages with open consonant-vowel syllables, and split long lines. Last resort: hyphenate the cluster (zmrz-li-na). |
| Word-final devoicing (led, lež, hrad, zub) | The final consonant goes voiceless: led = "let", lež = "leš", hrad = "hrat", zub = "zup" | Voiced the English way ("lezh"), which breaks rhymes that rely on sound, such as lež – keš | Usually leave the spelling alone, because it is correct Czech. If the rhyme audibly fails, rewrite the pair, or respell that word in the Suno lyrics only (lež → leš) and record it in Pronunciation Notes. |

### Stress Drift

Czech stress always falls on the **first syllable**. A one-syllable preposition usually takes the stress of a short word after it ("do domu" = DO-do-mu); before a longer word the stress may stay on the noun (na PAR-ko-viš-ti). The non-syllabic prepositions v, z, s, k add no syllable (v PRA-ze). This is standard Czech phonetics.

On the Suno side:
- **reported**: one v3-era case of a "Balkan" accent on "dokázáno" (Živě.cz). The source doesn't say which syllable took the stress.
- **untested**: Suno may stress the second-to-last syllable, the way Polish does, or follow the melody's accents wherever they fall.

| Word | Czech Stress | Drifted Stress | Sounds Like |
|------|--------------|----------------|-------------|
| ulice | **U**-li-ce | u-**LI**-ce | Polish stress on the second-to-last syllable |
| kamarád | **KA**-ma-rád | ka-**MA**-rád | A foreign accent |
| do domu | **DO**-do-mu | do-**DO**-mu | Preposition stress lost |

The capitals above are notation for this guide only. Don't put them in Suno lyrics.

**Fix by rewriting the line, not by marking it up:**
1. Place word-initial syllables, and prepositions before short nouns, on the strong beats (kick and snare). Rearrange the words until they land there: "ulice mě volá" puts **U** on the beat.
2. A long vowel can take a beat or a held note in a non-initial position without sounding wrong (pe-**NÍ**-ze). A short non-initial syllable on the snare cannot (u-**LI**-ce).
3. **Don't add accent marks.** In Czech the čárka means vowel length, not stress, so an extra mark changes the word. (Combining stress marks are reported to work for Russian (sunomarket), but that does not carry over.)
4. **Don't use caps to show stress.** Caps-for-stress is undocumented, and one vendor reports that caps make the delivery louder (HookGenius).
5. Split long lines (Jack Righteous, verified text).
6. If a well-written line still drifts, regenerate, because Suno is non-deterministic. For a single wrong word, use Replace Section; for a word that is right but unclear, use Remaster (Jack Righteous, verified text).

Full prosody and flow rules: [czech-craft.md](../../skills/lyric-writer/czech-craft.md).

### English Slang Inside Czech Lines

- **One language per line at minimum, one per section preferred.** The section rule above (§ Multilingual Tracks) still holds. The evidence that mixing within a line fails:
  - HookGenius reports that v5 still fails on mixed-language content (vendor claim).
  - One reader comment on the Jack Righteous multilingual guide (May 2026) says word-by-word switching is possible but "not easy and not always consistant".
  - The v3 "statisticky" case shows the contamination runs both ways.
- **English hooks go in their own section** (`[Hook]` or `[Chorus]`), following the K-pop pattern in [best-practices.md](best-practices.md). Run `check_homographs` on those English lines as usual. This is untested for Czech.
- **Inside Czech verses, spell slang the Czech way** so Suno applies Czech letter rules. This is **untested**; it builds on the reported Czech advice to write foreign words phonetically.

| English | Czech Spelling | Notes |
|---------|----------------|-------|
| cash | keš | Rhymes by sound with lež and běž |
| chill / chilling | čil / čilovat | Avoids the risky ch |
| flex / I flex | flex / flexím | flex is already phonetic for Czech; Czech endings make the verb |
| cool | kúl | |
| hype | hajp | |
| flow | flou | |
| OK | okej | |
| DJ | dýdžej | |
| MC | emsí | |

Keep each respelling identical everywhere it appears. In streaming and distributor lyrics, use the spelling the artist would publish. Note every respelling in Pronunciation Notes, and record both spellings when the two differ.

### Numbers & Abbreviations

**Write numbers and abbreviations out as Czech words.** The general rule in § Numbers applies. There is no Czech-specific data, and the guess that raw digits default to English readings is **untested**.

| Write | Not |
|-------|-----|
| jednadvacet *or* dvacet jedna | 21 |
| devatenáct set osmdesát čtyři | 1984 |
| dva tisíce dvacet čtyři | 2024 |
| sto korun | 100 Kč |
| čé er | ČR |
| emsí | MC |
| dýdžej | DJ |

Don't use the English `'93` shortcut in Czech lyrics. It invites an English reading, so write the year out in Czech.

### v6 Test Plan

The labels in this section only change when someone runs a test. Set up the test like this:
- Settings: Variety Off, Max Mode On.
- Generate each test line three ways: with diacritics, with diacritics stripped, and respelled.
- Have a native Czech speaker check every take.

Test words:
- **ř**: řeka, moře, tři, přes, dřív
- **ě**: věc, děti, mě, pět
- **ů**: dům, můj, půl
- **ch**: chci, chlap, ticho, prach, chata
- **c**: cena, ulice, cíl
- **clusters**: čtvrtek, prst, smrt, zmrzl
- **English-looking Czech words**: statisticky, problém, super, hit
- **loanwords**: beat, flow, cash, chill
- **numbers**: "21", "2024"
- **abbreviations**: ČR, DJ, OK

Record results here, with the date and model, and update each row's status.

### Sources (Czech Section)

Reddit and Discord could not be reached during research. None of these sources tests v6.

- [Suno — Introducing v6](https://suno.com/blog/introducing-v6) (9 Sep 2026; no language claims)
- [aifirst.cz — Suno průvodce](https://www.aifirst.cz/pruvodce/suno) (undated)
- [Písničky na křižovatce — Návod, jak pracovat s nástrojem Suno.ai](https://pisnickynakrizovatce.estranky.cz/clanky/tutorial/navod--jak-pracovat-s-nastrojem-suno.ai.html) (undated; mentions v1/v2)
- [Živě.cz — Česká hymna jako od Nirvany, rapová verze Máchova Máje](https://www.zive.cz/clanky/ceska-hymna-jako-od-nirvany-rapova-verze-machova-maje-generator-hudby-sunoai-musite-slyset-jinak-neuverite/sc-3-a-227303/default.aspx) (v3 era; known only from a search snippet)
- [Lupa.cz — Suno v3 launch](https://www.lupa.cz/aktuality/dvouminutove-pisnicky-o-cemkoli-ai-generator-hudby-suno-vydal-novou-verzi-pro-vsechny/) (26 Mar 2024)
- [VeŠkole.cz — Suno: nechte žáky skládat vlastní písničky](https://www.veskole.cz/clanky/suno-nechte-zaky-skladat-vlastni-pisnicky) (15 Oct 2024)
- [d3arts.cz — Suno návod](https://d3arts.cz/umela-inteligence/suno-navod-generovani-hudby-cesky-prompt-engineering/) (7 Jun 2026, v5.5)
- [tomoviny.cz — Jak na Suno](https://tomoviny.cz/jak-na-suno/) (2026)
- [Sunomarket — Suno songs in other languages](https://sunomarket.com/blog/suno-songs-other-languages) (undated; testing not stated)
- [HookGenius — Multi-language guide](https://hookgenius.app/guide/multi-language) and [Fix Suno pronunciation](https://hookgenius.app/learn/fix-suno-pronunciation/) (vendor)
- [Jack Righteous — Suno v5 multilingual pronunciation guide](https://jackrighteous.com/en-us/blogs/guides-using-suno-ai-music-creation/suno-v5-multilingual-english-pronunciation-guide) and [v5.5 pronunciation fix guide](https://jackrighteous.com/en-us/blogs/guides-using-suno-ai-music-creation/suno-v5-5-pronunciation-fix-guide-best-practices-for-wrong-or-unclear-lyrics)
- [promptowy.com — Suno AI po polsku](https://promptowy.com/suno-ai-po-polsku/) (2026-09-12; Polish analogue, no listening test)
- Suno song metadata: [Czech playlist (v4.5)](https://suno.com/playlist/2cca1f46-5a7a-41b4-9289-55bb947352ea), [Czech/Slovak playlist (v3.5)](https://suno.com/playlist/1119ae44-43b8-42cf-a542-c7696bbaba96)

---

## Quick Reference Card

```
HIGH-RISK WORDS (always check):
live, read, lead, wind, close, tear, bow, bass, wound

TECH TERMS (verify pronunciation):
- Compound brands: LiveJournal, YouTube, GitHub
- Acronyms: SQL, GUI, GIF, IEEE, ASCII
- Tech words: Linux, cache, daemon, router

FIX PRIORITY:
1. Rewrite (different word)
2. Phonetic spelling (looks weird, works)
3. Hyphenation (break syllables)
4. Context padding (add clarifying words)
5. Accept (document and move on)

DOCUMENT RISKS:
Add "Pronunciation Risks" section to Production Notes
if a word can't be fixed but might mispronounce.
```

## Accent Simulation

Suno doesn't have direct accent controls, but you can simulate accents:

### Technique

1. **Rewrite lyrics phonetically** as spoken in target accent
   - NOT dictionary spelling
   - Spell words as they sound in the accent

2. **Add accent name to style box**
   - Example: "Russian accent"
   - Example: "Jamaican accent"
   - Example: "Southern drawl"

3. **Use ChatGPT for conversion** (optional)
   - Prompt: "Rewrite these lyrics phonetically for a [accent] accent"

### Examples

**Standard**: "I'm going to the store"
**Russian accent**: "Ahm go-ink to da store"
**Jamaican accent**: "Mi ah go ah di store"
**Southern US**: "Ahm goin' to tha store"

**Note**: Results vary by accent complexity. Simple accents (Russian, Irish) work better than complex regional dialects.

---

## Testing

When in doubt:
1. Say the line out loud both ways
2. Ask: "If Suno picks wrong, is the song ruined?"
3. If yes, fix it. If no, document and move on.

---

## Related Skills

- **`/bitwize-music:pronunciation-specialist`** - Automated pronunciation scanning for lyrics
  - Scans for homographs, proper nouns, acronyms, tech terms
  - Uses this guide as reference
  - Suggests phonetic fixes automatically

- **`/bitwize-music:lyric-writer`** - Lyric writing with automatic pronunciation checks
  - Includes automatic pronunciation scanning after every draft
  - Applies rules from this guide during review process

- **`/bitwize-music:lyric-reviewer`** - Pre-generation QC gate
  - 13-point checklist includes pronunciation verification
  - Verifies homograph decisions and phonetic spelling application before Suno generation

## See Also

- **`/reference/suno/best-practices.md`** - Overall Suno prompting guide, style box construction
- **`/reference/suno/structure-tags.md`** - Section tags for organizing lyrics ([Verse], [Chorus], etc.)
- **`/skills/lyric-writer/SKILL.md`** - Complete lyric writing workflow and quality standards
- **`/skills/pronunciation-specialist/SKILL.md`** - Detailed pronunciation specialist skill documentation
- **`/skills/lyric-writer/czech-craft.md`** - Czech prosody, rhyme and flow rules (pairs with § Czech Pronunciation)
