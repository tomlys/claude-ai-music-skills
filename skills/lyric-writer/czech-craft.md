# Czech Lyric Craft Reference

Czech-language prosody, rhyme and flow rules for the lyric-writer skill, built for rap, trap and drill.
Read when a track's lyrics are in Czech (genre `czech-rap` or any Czech-language track).

---

## When to Apply

**Triggers**: the album genre is `czech-rap`, or any track's lyrics are wholly or partly in Czech.

**Still applies unchanged**:
- The 13-point check in [SKILL.md](SKILL.md). This file adds Czech checks to existing points (see [Per-Bar QA Checklist](#per-bar-qa-checklist)). It never adds a point.
- Section length limits in [craft-reference.md](craft-reference.md) → "Hip-Hop / Rap / Trap / Drill…": verse max 8 lines, hook 4–6.
- The `Density/pacing (Suno)` line in [genres/czech-rap/README.md](../../genres/czech-rap/README.md), or in the track's own genre README.
- Show don't tell, POV/tense, verse-chorus echo, hook and title placement.

**Replaced for Czech lines.** The English rules give wrong answers on Czech:

| English rule (SKILL.md / craft-reference.md) | Czech replacement in this file |
|-----------------------------------------------|--------------------------------|
| Prosody: lexical stress (HAP-py), stresses on beats 1 and 3 | [Stress-to-Beat Mapping](#stress-to-beat-mapping) |
| Rhyme types and rhyme quality | [Czech Rhyme Theory and Grading](#czech-rhyme-theory-and-grading) |
| Syllable counting; hip-hop line tolerance ±3 | [Syllable Counting and Bar Density](#syllable-counting-and-bar-density) (±2) |
| Word count targets (hip-hop 400–600) | [Word Count](#word-count) |
| Homograph table; invented-contraction rule | Czech spelling is near-phonemic, so the English homograph table does not apply to Czech lines. It still applies to English lines. Standard Czech contractions (šels, cos, sis) are fine. |

**Suno pronunciation** (diacritics, risky letters, slang spelling, numbers, Style Box wording) lives in [pronunciation-guide.md → Czech Pronunciation](../../reference/suno/pronunciation-guide.md#czech-pronunciation). This file covers what the writer controls on the page.

**Notation** (working notes only, never in the Suno Lyrics Box):

| Mark | Meaning | Example |
|------|---------|---------|
| CAPS | Stressed syllable | U-li-ce |
| `-` | Syllable boundary | ne-u-mím |
| `[ ]` | Pronunciation, written in Czech letters as heard (i and y both written i) | lež [leš], zpátky [spátki] |
| `·` | Rest (in grids) | |
| `~` | Held syllable (in grids) | |

In grids and code blocks, a vertical bar marks a stress-group boundary: `|DO-do-mu|`.

---

## Why Czech Is Different

| Area | English habit | Czech reality | What it means for the writer |
|------|---------------|---------------|------------------------------|
| Word stress | Varies by word (reCORD / REcord) | Always the first syllable | Put word starts on the beat; there is nothing to look up |
| Stress strength | Loud, long, high | Weak; it marks where a word begins | Czech tolerates syncopation. What sounds foreign is a non-initial syllable on a hard accent |
| Vowel length | Follows stress | Separate and meaningful (byt / být) | Long vowels can carry held notes in any position, but length does not make a syllable stressed. Lengths must match in rhymes |
| Syllable nuclei | Vowels only | Vowels, plus r and l (vlk, Brno) | Count syllables by hand |
| Consonant clusters | Mostly at word ends | Often at word starts (vzpomínky, čtvrť, zmrzlý) | Keep them out of fast passages |
| Inflection | Few endings | Seven cases and rich verb endings | Rhymes on endings are free and sound cheap (grade D) |
| Spelling | Irregular | Near-phonemic, with fixed sound rules | Rhyme by sound after applying the rules |
| Rhyme norm | One stressed syllable | Two syllables | The default end rhyme covers the last two syllables |

### Fixed First-Syllable Stress

- Stress falls on the first syllable of every word, including prefixes: NE-chci, PŘI-jdu, NEJ-lep-ší, VY-hrát, ZA-po-mněl, KA-ma-rád.
- Stress marks where a word begins. It does not separate the meanings of words, but the boundaries of stress groups can: |PRO-ti |VNĚJ-ším (against the outer ones) vs |PRO-tiv-něj-ším (more disgusting) (Skarnitzl 2014, after Palková); |ZA-se |DAL (gave again) vs |ZA-se-dal (sat in session).
- Czech stress is acoustically weak. The stressed syllable is often no louder or longer than the next one, and the syllable after it can even be more prominent (Volín and Skarnitzl, cited in Skarnitzl 2014). Listeners track where words start, not which syllable is loud.
  - Consequence: syncopated placement is fine.
  - The real error is a hard musical accent on a non-initial syllable while the first syllable is swallowed. u-LI-ce sounds Polish (Polish stresses the second-to-last syllable). ka-MA-rád sounds foreign.

### Vowel Length Is Separate from Stress

- Length changes meaning: byt (flat) / být (to be), pas (passport) / pás (belt), dal (gave) / dál (further), rada (advice) / ráda (glad, feminine), vila (villa) / víla (fairy).
- Long vowels often sit in unstressed syllables: KA-ma-rád, NÁ-dra-ží, ZA-hrád-ka.
- Long vowels are á é í ý ó ú ů, plus the diphthong ou.

### Syllabic R and L

Between consonants, or at a word end after a consonant, r and l act as vowels:
- one syllable: vlk, krk, smrt, prst, čtvrt;
- two syllables: Brno, srdce, čtvrtek, mrtvý, řekl, Petr;
- three syllables: Vltava;
- "Strč prst skrz krk" has four syllables.

### Consonant Clusters

Czech piles consonants at the start of words: vzpomínky [fspomínki], čtvrť, zmrzlý, scvrklý, nejsmutnější. Each cluster costs time. At rap speed it turns to mush.

### Spelling Is (Almost) Sound

Apply these before judging any rhyme:
- **i = y, í = ý**: mít and mýt are both [mít].
  - Exception: di/ti/ni soften the consonant, and dy/ty/ny do not. kosti [kosťi] vs mosty [mosti].
  - Loanwords: in most of them di/ti/ni stay hard [di ti ni] (rádio, pódium, titul, politika, kritika). Rhyme them by the hard sound.
- **ů = ú**: dům [dúm].
- **ě**:
  - bě/pě/vě/fě = [bje pje vje fje];
  - mě = [mňe], so mě and mně sound the same;
  - dě/tě/ně = [ďe ťe ňe].
- **Final consonants devoice**: led [let], lež [leš], hrad [hrat], krev [kref], sníh [sňích].
- **Clusters assimilate voicing**: kde [gde], zpátky [spátki], svatba [svadba], zahrádka [zahrátka].
- **ou, au, eu are single diphthongs**: ou rhymes only with ou (tou – mou, not tou – to).

### Rich Inflection Makes Cheap Rhymes Free

Thousands of words share each ending: every infinitive in -at, every verbal noun in -ání/-ení, every first-person verb in -ám/-ím, every instrumental plural in -ami/-ama.
- A rhyme carried only by such an ending is effortless, and Czech listeners hear it as lazy. Versology calls it *gramatický rým*.
- In Sgallová's punch-card study of F. J. Rubeš's 19th-century declamatory verse (*deklamovánky*), about 16% of rhymed lines were first-degree grammatical (only the ending rhymes: rukama – nohama) and 27–30% second-degree (the ending plus a rhyming stem sound: chodíme – vodíme). That ubiquity is why they sound cheap.

### The Rhyme Norm Is Two Syllables

- Czech treats the two-syllable (feminine) rhyme as normal: nebe – tebe, chleba – třeba.
- A one-syllable rhyme counts only when the line ends in a one-syllable word: noc – moc, svět – zpět.

---

## Stress-to-Beat Mapping

### Stress Groups

Czech stress belongs to the stress group (*mluvní takt*): a word plus any unstressed words leaning on it.

| Unit | Stress rule | Examples |
|------|-------------|----------|
| Word | First syllable | U-li-ce, NE-vím, KA-ma-rád |
| Prefix | Part of the word, so it takes the stress | PŘI-jdu, NEJ-lep-ší, VY-hrát, NE-u-mím |
| One-syllable preposition + noun | Usually the preposition takes the stress: about two-thirds of cases in read news and three-quarters in spontaneous speech (Skarnitzl 2014) | do domu = DO-do-mu; na stole = NA-sto-le; bez tebe = BEZ-te-be; do tmy = DO-tmy |
| One-syllable preposition, stress on the next word | The stress may move to the noun, making the preposition a pickup. Speakers do it to even out the rhythm and for emphasis, more often before longer words and before adjective + noun. Vowel length plays no part | do O-lo-mou-ce; na PAR-ko-viš-ti; na KRÁS-ném DU-na-ji; for rhythm or emphasis also na TRA-se |
| Non-syllabic preposition (v, z, s, k) | Adds no syllable; the group starts with the noun | v PRA-ze (2 syllables); s TE-bou; k NÁM (1 syllable); z DO-mu |
| Vocalized preposition (ve, ze, se, ke) | Adds a syllable and takes the stress | VE-měs-tě; ZE-sna; SE-mnou; KE-mně |
| Two-syllable preposition | Carries its own stress | KO-lem, ME-zi, BĚ-hem, KRO-mě |
| Enclitics (always unstressed) | Lean on the preceding stressed word | se, si, mi, ti, mu, ho, tě, mě; jsem, jsi, jsme, jste (past auxiliary and copula); bych, bys, by |
| Unstable enclitics | Stressed or not, depending on emphasis | je, to, tak, tam, teď, tu, už, prý, snad, asi |
| Words of 4+ syllables | A weak secondary stress around the 3rd syllable (practitioner heuristic) | ZA-po-MÍ-nám, NE-zá-VIS-lost, PŘI-pra-VE-ný |

The vocalized preposition "se" (with: SE-mnou) is stressed. The reflexive "se" is never stressed. Don't confuse them.

The copula jsem/jsi/jsme/jste ("am", "are"; spoken and in obecná written sem/seš/sme/ste) is unstressed too, but unlike the other enclitics it may open a clause: Jsem rád. Sem doma. See [Clitics: Second Position](#clitics-second-position).

### Clitics: Second Position

- **Position**: Enclitics sit in the second position of the clause, after the first stressed word or phrase.
- **Order**: auxiliary (jsem, bych) → reflexive (se, si) → dative (mi, ti) → accusative (ho, to). Examples: "Dal jsem ti ho." "Koupil jsem si to."
- **Never start a clause with se, si, mi, ti, mu, ho, tě, mě, bych/bys/by or the past auxiliary.**
  - ❌ "Jsem to udělal." → ✅ "Udělal jsem to."
  - ❌ "Mi je to jedno." → ✅ "Je mi to jedno."
  - ❌ "Koupil jsem to si." → ✅ "Koupil jsem si to."
- **Exceptions**:
  - The copula jsem/jsi/jsme/jste (sem/seš/sme/ste in obecná) may begin a clause: "Jsem rád." "Sem doma."
  - In obecná street register, a clause-initial se or si is real colloquial speech: "Se mi to nelíbí." "Si děláš srandu?" Use it only as a deliberate persona marker. In a standard or neutral verse write "To se mi nelíbí."
- **Enclitics are the best unstressed filler.** They sit right after a stressed syllable and never fight the beat: |ŘEK-la mi |PRAV-du.
- **Never rest a rhyme on an enclitic.** A line-final jsem, se or mi carries no stress, so it cannot carry a rhyme.
- **Contractions save a syllable and are acceptable in writing**: co jsi → cos ("Cos čekal?"), kde jsi → kdes, šel jsi → šels, jsi si → sis ("Co sis myslel?").

### Beat Rules

1. **Hard accents take group-initial syllables.** Every snare (felt beats 2 and 4 in half-time trap) and every kick or accented hit carries the first syllable of a stress group.
2. **Long vowels on held notes** (practitioner rule). In sung or melodic lines, or on a held line-final note, a non-initial long vowel (á é í ý ó ú ů, ou) may carry the note: ka-ma-RÁD~, zapomí-NÁM~. On a hard rapped accent mid-line it still sounds foreign (❌ pe-NÍ-ze on the snare), because Czech stress ignores vowel length. A short non-initial syllable never works: ❌ u-LI-ce, ❌ ka-MA-rád.
3. **Unstressed material fills the weak slots** (e, &, a): word tails, enclitics, conjunctions.
4. **Rhyme placement**:
   - Two-syllable rhyme word: stressed syllable on the snare, tail on the next slot.
   - One-syllable rhyme word: on the snare; hold it if the vowel is long.
5. **Prepositions**:
   - A one-syllable preposition is stressed by default (|DO tmy|).
   - It may instead be an unstressed pickup, with the stress on the first syllable of the noun: na |TRA-se|, na |SPLÁT-ky|, na |SCÉ-ně|, na |PAR-ko-viš-ti|. Czech speakers shift stress this way for even rhythm and for emphasis, whatever the vowel length, and more often before longer words. Both placements sound native.
   - What is forbidden is a non-initial syllable of the word itself on the accent (u-LI-ce).
6. **Pickups** (*předrážka*):
   - A line may start before beat 1 with unstressed material: a conjunction (a, že, ať, když), a particle, or a one-syllable preposition (rule 5).
   - Never start a pickup with the first syllable of a longer word whose second syllable then lands on the beat. That is the u-LI-ce error.

### The Half-Time Trap Grid

Trap is programmed at 130–150 BPM but felt at half time (65–75 BPM), with the snare on felt beats 2 and 4.
- **Unit**: one felt bar = two programmed bars, about 3.4 s at 140 BPM.
- **Grid**: 16 sixteenth-note slots at the felt tempo.
- **Written line**: one felt bar. That is why an 8-line verse is the "16-bar verse" of craft-reference.

The grid is a writing tool for placing stresses. Suno does not read it and sets its own timing. What Suno responds to is line length, line count and line breaks (see [Bar Density by Tempo](#bar-density-by-tempo)).

The opening couplet of the [worked example](#worked-example-8-bar-verse), on the grid (the full verse is gridded there):

```
felt beat  1                   2                   3                   4
slot       1    e    &    a    2    e    &    a    3    e    &    a    4    e    &    a
drums      K                   S                   K                   S
L1         ZI   ma   jak  ·    PRA  se   KAP  se   NO   vá   ·    ·    ZPRÁ ~    va   ·
L2         NA   skla dě   ·    ZA   se   JE   nom  HOR  ká   ·    ·    KÁ   ~    va   ·
```

- **L1** "Zima jak prase, v kapse nová zpráva" (11 syllables). The v of "v kapse" merges into KAP and adds no syllable.
- **L2** "na skladě zase jenom horká káva" (11 syllables). In "na skladě", NA keeps the default preposition stress and takes beat 1.
- **Snares**: every snare carries a stressed syllable. Beat 2 carries the internal rhyme (PRA-se / ZA-se). Beat 4 carries the end rhyme (ZPRÁ-va / KÁ-va).
- **Beats 1 and 3**: also stressed syllables. No non-initial syllable sits on any beat.
- **Weak slots**: long vowels on weak slots (vá, ká) are fine. Length is not stress.

### Worked Fixes

**Wrong syllable on the snare.** "Tahle ulice mě zná" (7 syllables):

```
slot       1    e    &    a    2    e    &    a    3
drums      K                   S                   K
wrong      TAH  le   u    ·    LI   ce   mě   ·    ZNÁ
right      ·    ·    TAH  le   U    li   ce   mě   ZNÁ
```

- ❌ **wrong**: the short, non-initial LI lands on the snare, which reads as u-LI-ce.
- ✅ **right**: the line starts two slots later. U lands on the snare, the enclitic mě fills a weak slot, and ZNÁ takes beat 3.

**Preposition before the rhyme word.** "…žít na splátky" against "…jedu zpátky":
- By default "na" takes the stress (NA splát-ky). On the grid that would push the rhyme one slot late.
- Fix: make "na" a pickup so SPLÁT lands on the snare, level with ZPÁT (beat rule 5). The same works for "na trase" against "zase": jsem zase na |TRA-se| with TRA on the snare sounds native.
- Or keep NA on the snare and let the rhyme fall one slot late. Pick one and keep it consistent across the couplet.

**Long vowel saves a line end.** "To je můj kamarád":
- Rapped with KA on the snare, it is natural.
- Sung with the long RÁD held on the final snare, it also works (rule 2). A hard, short rapped hit on RÁD does not.
- Never put the short MA on the accent.

---

## Czech Rhyme Theory and Grading

### The Rhyme Domain

The rhyme domain is the part of the end word that must match:
- **End word of 2+ syllables**: from the vowel of the second-to-last syllable to the end. zprá-va → [áva]; pa-le-ty → [eti]; stra-chy → [achi].
- **End word of one syllable**: its vowel and the consonants after it. noc → [oc]; dál → [ál].
- **One-syllable end word against a longer one**: compare the last syllables only, and treat the pair as stress-misaligned (see below), unless the longer word's last syllable has a long vowel held at the line end (beat rule 2: rád / kamarád~, both [át]).

Compare domains **by sound** (see [Spelling Is (Almost) Sound](#spelling-is-almost-sound)), not by letters.

### Clean and Rich

- **Clean rhyme**: the domains match exactly — vowel quality, vowel length and every following consonant, by sound.
- **Rich rhyme** (this file's meaning of *bohatý rým*): a clean rhyme whose consonant immediately before the first rhyming vowel also matches (the *opěrná souhláska*). tělo – chtělo shares [ťelo]; brána – rána shares [rána].
  - Czech versology uses *bohatý* in more than one sense. Some sources call any clean rhyme *bohatý*. In this file it always means the supporting-consonant version.
  - The glide that ě adds after b, p, v, f ([j]) and m ([ň]) is not a supporting consonant on its own. Compare the consonant before it: svět – zpět (v / p) is B; světa – věta (v / v) is A2.

### Stress Alignment

A rhyme is **stress-aligned** when both domains sit in the same position relative to the stress:
- both start on the stressed syllable (ZPRÁ-va / KÁ-va); or
- both start one syllable after it (PA-le-ty / PŘED le-ty; POS-ta-va / VL-ta-va).

A one-syllable preposition before the rhyme word can go either way ([beat rule 5](#beat-rules)). Used as a pickup, it leaves the noun's first syllable stressed, so ZPÁT-ky / na SPLÁT-ky and ZA-se / na TRA-se are aligned.

A misaligned rhyme (RU-ce / ka-PU-ce) forces one line either to put a non-initial syllable on the snare or to slide its rhyme off the beat. **Misaligned → one grade lower.**

### Stem or Ending

Decide what carries the matching domain:
- **The stem** (part of the word's root): fine. tělo – chtělo, cesta – města.
- **Only an inflectional or derivational ending**, with nothing from the stem: grammatical rhyme, grade D. milovat – pracovat (-ovat), volání – čekání (-ání), chodíme – mluvíme (-íme).
- **The same ending on two different stems is fine when the domain reaches into the stems.** noci – moci ([oci]: noc-/moc- + -i), slávu – zprávu ([ávu]).
- **A domain made only of the ending, with rhyming stems to its left** (cho-DÍ-me / vo-DÍ-me: the domain [íme] is all ending, but chod-/vod- rhyme): not D, because the stems join in. It is still a stock same-form pair, which Czech versology counts as grammatical rhyme of the second degree (Sgallová 2015). Grade it **B at most**, and keep it out of hooks and punchlines.

### Grade Scale

| Grade | Name | Definition | Verdict |
|-------|------|------------|---------|
| **A** | Multi or rich | **A1 multi (vícerým)**: 3+ matching vowels in sequence, stress-aligned, ending in a clean two-syllable rhyme. **A2 rich**: a clean, stress-aligned rhyme that also matches the supporting consonant, carried by different stems, ideally across word classes or forms | Use for hooks, punchlines and closing couplets |
| **B** | Clean | A clean, stress-aligned rhyme carried by the stem: feminine for 2+-syllable end words, masculine between two different one-syllable content words | Default end rhyme |
| **C** | Weak | Assonance only (vowels match, consonants differ); a length mismatch on the first rhyming vowel; a final-vowel length mismatch (B → C); a stress-misaligned clean rhyme (B → C); a one-syllable word against a longer one, unless the longer word's long final vowel is held | Internal rhyme only, with one exception (see policy) |
| **D** | Grammatical | The match comes only from an ending (-at, -ovat, -ání/-ení, -ám/-ím, -íme, -ách, -ama, -ou, -em, -ej) and nothing to its left rhymes; or the words differ only by a prefix of the same lexeme (hrát – prohrát); or homophones (být – bít) used as a rhyme | **Reject** and rewrite |
| **X** | Identical | The same word rhymed with itself (noc – noc) | **Reject** and rewrite |

Downgrades stack. A final-vowel length mismatch on an otherwise A2 pair makes it B.

### End-Rhyme Policy

| Position | Allowed grades |
|----------|----------------|
| Hook / chorus end rhymes | A or B only |
| Verse end rhymes | A or B. C is allowed only as a stress-aligned assonance multi of 4+ vowels (dneska v noci / ze sna do tmy), at most one such couplet per 8-line verse |
| Internal rhymes and chains | A, B or C |
| Anywhere | Never D or X as a deliberate rhyme. A pun on near-homophones is fine when the meanings clearly differ and it is not the end rhyme |

### Grade A Examples

| Pair | Sound check | Why A |
|------|-------------|-------|
| nová zpráva / horká káva | NO-vá ZPRÁ-va / HOR-ká KÁ-va: o-á-á-a both | A1: four-vowel multi, stress-aligned, clean [áva] |
| nechci slávu / nejsi v právu | NECH-ci SLÁ-vu / NEJ-si v PRÁ-vu: e-i-á-u both | A1: four-vowel multi; accusative slávu vs locative v právu |
| nemám prachy / neumírám strachy | NE-mám PRA-chy / NE-u-mí-rám STRA-chy: unstressed á, stressed a, unstressed i in both | A1 and A2: three-vowel multi plus the supporting r ([rachi]) |
| mám zlato / dáš za to | MÁM ZLA-to / DÁŠ ZA to: á-a-o both | A1: mosaic multi across a word boundary |
| město svítí / co kdo cítí | MĚS-to SVÍ-tí / CO kdo CÍ-tí: unstressed o, stressed í, unstressed í | A1: three-vowel multi, clean [íťí] |
| světa – věta | [svjeta] / [vjeta] | A2: the whole [vjeta] is shared; genitive of svět vs a different noun |
| tělo – chtělo | [ťelo] / [chťelo] | A2: supporting ť; noun vs verb |
| zrada – brada | [zrada] / [brada] | A2: supporting r; unrelated stems |
| brána – rána | [brána] / [rána] | A2: supporting r. These are unrelated words, so this is not a prefix rhyme |
| postava – Vltava | [postava] / [vltava] | A2: supporting t; both domains start one syllable after the stress |
| palety – před lety | [paleti] / [leti] | A2: supporting l; both domains start one syllable after the stress; different stems |

### Grade B Examples

| Pair | Sound check | Note |
|------|-------------|------|
| noc – moc | [noc] / [moc] | Masculine; noun vs adverb |
| den – ven | [den] / [ven] | Masculine; noun vs adverb |
| svět – zpět | [svjet] / [spjet] | Masculine; noun vs adverb. The ě glide is not a supporting consonant (v / p), so not A2 |
| dál – stál | [dál] / [stál] | Masculine; long á in both |
| krev – zpěv | [kref] / [spjef] | Final v devoices to f in both |
| sníh – hřích | [sňích] / [hřích] | Final h devoices to ch |
| keš – lež | [keš] / [leš] | Final ž devoices to š |
| chleba – třeba | [chleba] / [třeba] | Noun vs particle |
| voda – škoda | [voda] / [škoda] | |
| cesta – města | [cesta] / [mňesta] | |
| v hlavě – zdravě | [hlavje] / [zdravje] | Noun vs adverb |
| káva – dává | [káva] / [dává] | Noun vs verb |
| zase – v hlase | [zase] / [hlase] | v adds no syllable, so both stress the first syllable |
| zpátky – na splátky | [spátki] / [splátki] | Aligned when na is a pickup (beat rule 5) |
| Praha – drahá | [praha] / [drahá] | A2 (supporting r) minus the final-vowel length mismatch → B |
| noci – moci | [noci] / [moci] | Same ending -i, but the stems noc-/moc- carry the rhyme |
| zlato – za to | [zlato] / [zato] | Mosaic; extend leftwards for A (mám zlato / dáš za to) |
| nebe – tebe | [nebe] / [tebe] | Technically B, but it is the most worn-out pair in Czech pop, the local moon/June. Treat it as a cliché |

### Grade C Examples

| Pair | Sound check | Why C |
|------|-------------|-------|
| hlava – sláva | [hlava] / [sláva] | Length mismatch on the first rhyming vowel |
| hrad – brát | [hrat] / [brát] | Length mismatch on the only vowel |
| Bůh – kruh | [búch] / [kruch] | ů is long |
| zrada – ráda | [zrada] / [ráda] | Length mismatch on the first rhyming vowel |
| lidi – vidí | [liďi] / [viďí] | Final-vowel length mismatch: B → C |
| chata – zlatá | [chata] / [zlatá] | Final-vowel length mismatch: B → C |
| kosti – mosty | [kosťi] / [mosti] | ti is soft, ty is hard |
| kapse – zase | [kapse] / [zase] | Consonants differ (ps / s): assonance |
| život – pivo | [život] / [pivo] | Vowels i-o only |
| kluci – Gucci | [kluci] / [guči] | c vs č |
| ruce – kapuce | RU-ce / ka-PU-ce | Clean, but misaligned (short pu): B → C |
| cesta – nevěsta | CES-ta / NE-věs-ta | Clean, but misaligned (short věs): B → C |
| zpátky – pohádky | ZPÁT-ky / po-HÁD-ky: [spátki] / [pohátki] | Clean (d becomes t before k), but misaligned in rapped flow: B → C. Only in a sung line with HÁD held can it pass as B (beat rule 2) |
| noc – nemoc | [noc] / [nemoc] | One-syllable word against the short final syllable of a longer word |
| dneska v noci / ze sna do tmy | DNES-ka v NO-ci / ZE sna DO tmy: e-a-o-i both | Assonance multi. It is the one C allowed at a verse line end |

### Grade D and X Examples (Reject)

| Pair | What carries the match | Grade |
|------|------------------------|-------|
| dělat – volat | Second-to-last vowels differ (e / o); only the infinitive ending -at matches | D |
| milovat – pracovat | The suffix -ovat | D |
| volání – čekání | The verbal-noun suffix -ání | D |
| trápení – mluvení | The verbal-noun suffix -ení | D |
| dělám – volám | Second-to-last vowels differ (ě / o); the match is the first-person -ám | D |
| mluvím – nosím | Only -ím matches; the vowels and consonants before it differ | D |
| chodíme – mluvíme | Only the ending -íme matches; the stems chod-/mluv- do not rhyme | D |
| s klukama – s holkama | The colloquial instrumental -ama | D |
| v horách – po stranách | The locative -ách | D |
| rukou – holkou | The instrumental -ou; second-to-last vowels differ (u / o) | D |
| domem – městem | The instrumental -em | D |
| velkej – malej | The colloquial adjective ending -ej | D |
| mám to v sobě / dám to tobě | Looks like a multi, but nothing in it is a free choice. sobě/tobě are two forms of the pronoun paradigm that differ only in s/t, so the end match is all case ending; to is the same word twice; mám/dám is a stock same-form verb pair | D |
| hrát – prohrát, jít – přijít, dělat – udělat, moc – pomoc | Same lexeme, different prefix | D |
| být – bít, mýt – mít, led – let | Homophones. Use only as a deliberate pun, never as the rhyme | D |
| noc – noc | Identical word | X |

The prefix test is about the morpheme, not the letters. brána – rána are unrelated words and rhyme richly (A). hrát – prohrát are one verb (D).

chodíme – vodíme is not in this table: its stems rhyme too, so it is a capped B (see [Stem or Ending](#stem-or-ending)). Sgallová (2015) counts it as second-degree grammatical rhyme; Hrabák (1958) had classed the type as split rhyme (*rým štěpný*), whose stem rhymes.

### Grading Procedure

Run this on every end-rhyme pair, and on internal rhymes you want to count:

1. **Convert to sound.** Write the last two syllables of each line in sound, applying [Spelling Is (Almost) Sound](#spelling-is-almost-sound).
2. **Find the domains.** See [The Rhyme Domain](#the-rhyme-domain).
3. **Compare the first rhyming vowel.** Quality and length must match. If they don't, it is C at best (assonance), or not a rhyme at all.
4. **Compare everything after it.** Consonants must match by sound, or it is C (assonance). The final vowel must match in quality; a length mismatch on it downgrades one step.
5. **Check what carries the match.** Ending only, meaning nothing to the left of the ending rhymes → D. Prefix only, or homophones → D. Same word → X. Stop here and rewrite. If the domain is all ending but the stems to its left rhyme too (chod-/vod-), continue, but cap the final grade at B.
6. **Check stress alignment.** Misaligned → downgrade one step.
7. **Check for a supporting consonant.** If it matches, and the stems are different → A2.
8. **Extend leftwards.** If 3+ stress-aligned vowels match and steps 3–6 passed → A1.
9. **Otherwise** it is B.
10. **Check the policy.** Compare the grade against the [End-Rhyme Policy](#end-rhyme-policy).

---

## Vícerýmy, Internal Rhyme and Assonance Chains

*Vícerým* (also *dvojrým*, *trojrým*) is scene usage for a multisyllabic rhyme. No standard Czech source defines it; this file uses it as practitioners do.

### Building a Multi

1. **Anchor**: write a strong two-syllable end rhyme first (B or better).
2. **Skeleton**: write the vowel skeleton of the last 3–5 syllables and mark the stresses. Example: "nová zpráva" = O-á-Á-a.
3. **Generate**: find phrases that match the skeleton and the stress positions. Word boundaries can fall anywhere (mosaic rhyme), but stressed syllables must land in the same positions.
4. **Lengths**: match length on stressed and held vowels. A short/long mismatch on an unstressed vowel inside the multi is tolerated.
5. **Sense first**: check meaning and grammar before the grade. A perfect multi that says nothing fails failure mode 7 ([Rhyme-driven nonsense](#common-failure-modes-of-ai-written-czech-lyrics)).

### Worked Builds

**Build 1. Anchor "nová zpráva" (O-á-Á-a, ends [áva]).**

| Candidate | Skeleton | Verdict |
|-----------|----------|---------|
| dobrá zpráva | O-á-Á-a | ❌ X: zpráva is the identical word |
| stará pravda | A-á-A-a | ❌ Stressed vowels differ (a vs o; short a vs long á), and [avda] ≠ [áva] |
| horká káva | O-á-Á-a | ✅ A1: same skeleton, same stresses, clean [áva] |

**Build 2. A whole couplet around "nechci slávu" (E-i-Á-u).**
```
Dělám to pro sebe, nechci slávu,       (10)
a jestli myslíš opak, nejsi v právu.   (11)
```
- NECH-ci SLÁ-vu / NEJ-si v PRÁ-vu: four vowels, both stresses aligned, clean [ávu] → **A1**.
- "být v právu" is the idiom for "to be in the right".

**Build 3. Mosaic across word boundaries.**
```
Na krku mám zlato,     (6)
kolik mi dáš za to?    (6)
```
- MÁM ZLA-to / DÁŠ ZA to: Á-A-o in both, so two words rhyme with three → **A1**.
- "krku" is kr-ku: the syllabic r counts.

### False Multis

Parallel grammar can fake a multi. In "mám to v sobě / dám to tobě", every matching sound comes from a repeated function word (to), the pronoun paradigm (sobě/tobě), or a stock same-form verb pair (mám/dám). Grade it **D** and rewrite.

Test: delete every ending and every function word. If the end pair no longer rhymes (sobě/tobě → s / t), the multi was fake.

### Internal Rhyme Placement

The hip-hop convention expects internal rhyme ([genres/hip-hop/README.md](../../genres/hip-hop/README.md)). Three placements work in Czech:

1. **Beat-aligned echo**: rhyming syllables land on the same beat in consecutive lines. In the [grid](#the-half-time-trap-grid), PRA-se (L1) and ZA-se (L2) both sit on beat 2 (B, clean [ase]).
2. **Ladder**: the end of one phrase rhymes with the start of the next line: "Tahám **palety**, bolí celý tělo, / **před lety** sem žil…" (A2, [leti]).
3. **Line-internal chain**: the same vowel pair on successive beats inside one line.
   ```
   Roky letí, kroky vedou do tmy.     (10)
   RO-ky LE-tí, KRO-ky VE-dou DO tmy
   ```
   o-i lands on beats 1, 2 and 3 in straight 16ths. roky – kroky is rich (supporting r); do tmy extends the chain by assonance.

### Assonance Chains

Assonance (*asonance*, *polorým*) matches vowels while the consonants differ. It is the backbone of modern rap density.
- Build chains from stressed syllables. A chain of unstressed endings is a grammatical rhyme in disguise.
- Example: "Zima jak **pra**se, v **kap**se nová zpráva, / na skladě **za**se jenom horká káva."
  - a-e hits on prase, kapse, zase.
  - prase – zase is a clean B.
  - kapse joins by assonance (C).
- A chain decorates. The hook's end rhyme still needs a clean final two syllables (A or B).

### Slang Rhyme Families

These are verified by sound. Pronounce loans the Czech way.

| Sound | Words | Note |
|-------|-------|------|
| [-eš] | keš, lež, běž, věž | ž devoices to š. Not seš: it is normally an unstressed clitic and cannot carry the rhyme |
| [-ip] | drip, vtip, typ | vtip = [fťip] |
| [-us] | čus, kus, plus, bus | |
| [-ít] | beat [bít], žít, mít, štít | Only if beat is sung the Czech way. cit [cit] is short, so it is C |
| [-rt] | smrt, zmrd [zmrt], čtvrt | smrt – zmrd is rich (supporting m). Explicit; set the Explicit flag |
| [-achi] | prachy, strachy | prachy = cash (plural only); strachy as in "umírat strachy" |
| [-áva] / [-ávu] | zpráva, káva, tráva, sláva / zprávu, trávu, slávu, právu | Not hlava or hlavu: short a, so C |
| [-eks] | flex, sex | Explicit content for sex depends on context |

---

## Syllable Counting and Bar Density

### Counting Rules

| Rule | Examples | Count |
|------|----------|-------|
| Every vowel letter is one syllable nucleus (a e ě i y o u, á é í ý ó ú ů) | ulice | 3 |
| ou, au, eu inside a morpheme = one syllable | pouze, auto, euro | 2, 2, 2 |
| Across a prefix boundary the vowels are separate | po-u-čit, ne-u-mím, do-u-čit | 3, 3, 3 |
| Vowel sequences in loanwords are separate | pó-di-um, rá-di-o | 3, 3 |
| Syllabic r/l between consonants or at a word end after a consonant | vlk, smrt, čtvrt / Brno, srdce, čtvrtek, řekl, Petr / Vltava | 1 / 2 / 3 |
| r/l next to a vowel is not syllabic | barva, Karel | 2, 2 |
| Final -e is always pronounced | hele, ale, Praze | 2, 2, 2 |
| ě is a vowel | město, věc | 2, 1 |
| -ej, -aj, -ůj are vowel + j, one syllable | dob-rej, dě-laj, můj | 2, 2, 1 |
| v, z, s, k as prepositions add no syllable | v Praze, s tebou, k nám, z domu | 2, 2, 1, 2 |
| ve, ze, se, ke add one | ve městě, se mnou, ze sna, ke mně | 3, 2, 2, 2 |

### Practice Set

| Text | Syllables | Breakdown |
|------|-----------|-----------|
| Přišel jsem | 3 | při-šel jsem |
| neumírám | 4 | ne-u-mí-rám |
| nejsmutnější | 4 | nej-smut-něj-ší |
| Strč prst skrz krk | 4 | strč prst skrz krk |
| dneska v noci | 4 | dnes-ka v no-ci |
| na pódiu | 4 | na pó-di-u |
| řekl / řek | 2 / 1 | ře-kl / řek |
| dělají / dělaj | 3 / 2 | dě-la-jí / dě-laj |
| nějaký / ňákej | 3 / 2 | ně-ja-ký / ňá-kej |
| s kluky / s klukama | 2 / 3 | s klu-ky / s klu-ka-ma |

### Don't Trust the MCP Syllable Tools on Czech

The server's lyric tools use English heuristics:
- `count_syllables`, `analyze_readability`, `analyze_rhyme_scheme` and `extract_distinctive_phrases` in `handlers/lyrics_analysis.py`;
- `check_cross_track_repetition` in `handlers/text_analysis.py`.

On Czech they fail in two ways:
- **Tokenizer**: `_WORD_TOKEN_RE = [a-zA-Z']+` (`handlers/_shared.py`) splits words at every diacritic. "Přišel" becomes p / i / el, "fér" becomes f / r, and "čtvrtek" loses its č.
- **Syllable heuristic**: `_count_syllables_word` counts English vowel groups and drops a final e. Measured:
  - ulice = 2 (really 3)
  - hele = 1 (really 2)
  - Brno = 1 (really 2)
  - pouze = 1 (really 2)
  - čtvrtek = 1 (really 2)
  - "dneska v noci" = 5 (really 4, because it counts the preposition v)

Count Czech lines by hand with the rules above. Treat those tools' syllable counts, rhyme groups, readability scores and repetition hits on Czech as unreliable.

### Bar Density by Tempo

Each written line is one felt bar. For half-time trap and drill, that is two programmed bars.

| Delivery | Programmed BPM | Felt BPM | Slots per line | Syllables per line | Lines per verse (Suno) |
|----------|----------------|----------|----------------|--------------------|------------------------|
| Boom bap, 16th-note rap | 85–95 | 85–95 | 16 | 10–14 | 8 default; max 6 at 80–85 BPM |
| Half-time trap, rapped 16ths | 130–150 | 65–75 | 16 | 10–14 | 8 default; 6 if the Musical Direction says slow or spacious |
| Half-time trap, melodic | 130–150 | 65–75 | 8 | 6–10 | Max 6 at ≤75 felt BPM |
| Triplet flow | 130–150 | 65–75 | 12 (four groups of three) | 10–12 | 8 |
| Drill | 140–145 | 70–72 | 16, with deliberate rests | 9–13 | 8, never more |

**Where these numbers come from**:
- The 8-line cap and the BPM bands follow [genres/czech-rap/README.md](../../genres/czech-rap/README.md), [genres/trap/README.md](../../genres/trap/README.md), [genres/drill/README.md](../../genres/drill/README.md) and [genres/boom-bap/README.md](../../genres/boom-bap/README.md).
- The two trap rows reconcile two READMEs. The trap README's "8–10 per bar" describes the spacious, melodic default; the czech-rap README's 10–14 describes a rapped 16th-note flow. Pick the row that matches the Musical Direction.

**Rough speeds** (approximate):
- One felt bar at 140 BPM is about 3.4 s, so 12 syllables is about 3.5 syllables per second.
- Ordinary Czech speech runs at roughly 5–6.
- Double-time 16ths at 140 BPM (about 9 per second) are bursts only, never a whole verse.

**Clusters cost time.** For cluster-heavy lines, aim at the low end of the band. Long lines make Suno rush, swallow consonants and misplace stress ([Czech Pronunciation](../../reference/suno/pronunciation-guide.md#czech-pronunciation)).

### Pairing Tolerance

- Rhyming partner lines stay within **±2 syllables**, and the rhyme lands on the same subdivision. This is stricter than the generic hip-hop ±3, because Czech's longer words make big swings audible.
- Verse 1 and Verse 2 line lengths should match, as in craft-reference.

### Word Count

Czech packs more syllables into each word. A 10–14-syllable rap line holds about 6–7 Czech words (estimate from the worked example: 52 words in 8 lines). The English hip-hop band of 400–600 words would therefore mean far too many lines.

- **Czech band**: a 3:30–5:00 Czech rap track usually lands around **250–350 words** (3 verses of 8 lines, plus hooks and a bridge). This is a practitioner estimate.
- **The 600-word cap in check 8 almost never fires on Czech.** If a Czech draft passes about 400 words, it almost certainly has too many lines. Recount against checks 9 and 11.
- **The under-200 flag** still makes sense.
- **`get_lyrics_stats` has no `czech-rap` entry** in `_GENRE_WORD_TARGETS` (`handlers/text_analysis.py`), so it falls back to the default 150–350. Its word count is a plain whitespace split, so the count itself is accurate on Czech; only the 150–350 target band is generic. Judge the count against the Czech band above.

---

## Flow Patterns

### Straight 16ths

One syllable per sixteenth at the felt tempo, with rests to breathe.
- Stressed syllables on beats 1–4.
- Optional extra accents on the "&".
- Rhyme on beat 4 (the second snare).

See the [grid](#the-half-time-trap-grid).

### Triplet Flow

Triplet flow places syllables in groups of three. It rose with slow trap beats (Duinker 2019). Czech fits it naturally, because every stress group starts with its stressed syllable: a three-syllable group starts on the triplet's strong slot by default.

```
triplet slot  1    .    .    2    .    .    3    .    .    4    .    .
right         ZA   pla  tím  NÁ   jem  a    DLU  hy   mi   ZŮ   sta  nou
wrong (+a)    a    ZA   pla  tím  NÁ   jem  a    DLU  hy   mi   ZŮ   sta   (nou spills)
```

- ✅ **right**: "Zaplatím nájem a dluhy mi zůstanou" (12 syllables): every group starts on a stressed syllable. The enclitic mi sits correctly after "dluhy".
- ❌ **wrong (+a)**: adding one syllable at the front ("A zaplatím…") pushes every stress onto a weak slot. One stray syllable wrecks a triplet line.

| Group shape | Example | Fit |
|-------------|---------|-----|
| Three-syllable word | PE-ní-ze, U-li-ce, ZA-pla-tím, KA-ma-rád, NÁ-dra-ží | ✅ Ideal |
| Two-syllable word + enclitic or conjunction | ŘEK-la mi, DLU-hy mi, NÁ-jem a | ✅ |
| Preposition + two-syllable noun | DO kap-sy, ZA ro-hem | ✅ |
| One-syllable word + two-syllable word | MÁM PRA-chy | ⚠️ The second stress lands on the weak middle slot; use the monosyllable as a pickup instead |
| Two-syllable word + one-syllable word | TĚŽ-ký DEN | ⚠️ The stress lands on the weakest slot; OK only at a line end |
| Four-syllable word | ZA-po-mí-nám | ⚠️ It spills into the next group. Split it so the next group starts on a new word, or end the line on a held nám |

**Speed**:
- Relaxed triplets (three per felt beat) run at about 3.5 syllables per second.
- Fast triplets (three per programmed beat at 140 BPM) run at about 7 per second.
- Either way, write the line as 12 slots and 10–12 syllables. The style prompt is the likelier lever for which speed Suno chooses (untested).

### Off-Beat Starts and Pickups

- **Starting on beat 1** sounds square.
- **Starting off the beat** sounds modern.
  - Begin with an unstressed pickup: že, a, ať, když, a one-syllable preposition before its noun ([Beat Rules](#beat-rules), rule 5), or "že prej".
  - The next stressed syllable must still land on a beat.
- **What a pickup can't be**: the start of a longer word ([Beat Rules](#beat-rules), rule 6).

### Rests and Stop-Start

- **Leave room for the rhyme**: a rest on the slot before the rhyme word makes it land harder.
- **A rest can sit on a snare.** An empty snare is better than a non-initial syllable on it.
- **Stop-start lines** end on a stressed monosyllable (DÁL, NIC, SÁM) followed by a rest. They suit drill.
- **Breathe**: a line break is a breath ([100-expert-tips.md](../../reference/suno/100-expert-tips.md) #29). In fast verses, end a sentence at a line break at least every two lines; a sentence running over many lines invites Suno to rush (untested for Czech).

### Melodic Trap and Held Notes

- **Hold long vowels**: á é í ý ó ú ů, ou. Good held words: dál, sám, já, ráno, zpátky, domů, tmou.
- **Don't hold short vowels in words with a long twin.** Stretching byt toward být, pas toward pás, or rada toward ráda blurs the meaning. End sung lines on long-vowel words where you can.
- **ř on a held note** is a pronunciation risk ([Czech Pronunciation](../../reference/suno/pronunciation-guide.md#czech-pronunciation)). Keep it off sustained notes.

### Hooks

- **Length**: 2–4 lines (6 at most). Repetition is a feature. AAAA rhyme and hooks built from one line repeated are normal in trap.
- **Rhyme**: A or B end rhymes only.
- **Title word**: put its stressed first syllable on a snare, and repeat the title in the first or last hook line.
- **English hooks** go in their own `[Hook]` section, never mixed into a Czech line.

### Clusters at Speed

- Words like vzpomínky, čtvrtek, zmrzlý, scvrklý and nejsmutnější belong after a rest, on a held note, or in slow passages.
- In fast 16ths or triplets, swap them for open consonant-vowel words. For example: vzpomínky → to, co bylo; ve čtvrtek → ten den.

---

## Register: Spisovná vs Obecná Čeština

**Spisovná čeština** (standard Czech) is the written, formal norm. **Obecná čeština** (common Czech) is the everyday Bohemian colloquial language and the genre norm for street rap, trap and drill. Czech RapCor Boosted (Czech RCB), a corpus of 7,211 Czech rap songs, is full of forms like chtěj, cejtim and vole.

| Feature | Spisovná | Obecná | Syllables |
|---------|----------|--------|-----------|
| ý → ej | dobrý, být, týden | dobrej, bejt, tejden | Same |
| é → í/ý | mléko, dobré pivo | mlíko, dobrý pivo | Same |
| Prothetic v- before o- | okno, on | vokno, von | Same (sounds rough; use sparingly) |
| Forms of být | jsem, jsi, jsou | sem, seš (or si), sou | Same |
| 3rd person plural | dělají, chtějí | dělaj, chtěj | −1 |
| Instrumental plural | s kluky, s lidmi | s klukama, s lidma | +1 / same |
| Past tense after a consonant | řekl, mohl, nesl | řek, moh, nes | −1 |
| Shortenings | nějaký, jestli, vždycky, ano, půjdu | ňákej, esli, dycky, jo, pudu | −1 / same |
| Conditional | bychom | bysme | Same |

**Rules**:
- **One register per song**, or per persona in a duet. Never switch between jsem and sem, or dobrý and dobrej, at random. A spisovná-only form in an obecná verse sticks out (❌ "Sem unavenej a nemohu spát" → ✅ "Sem unavenej a nemůžu spát").
- **Spelling**: if the song is written in obecná, write sem/seš/sou. sem and sou are how jsem and jsou are pronounced anyway; seš is the colloquial form of jsi as a full verb (seš borec), while jsi itself is spoken [si] and the past auxiliary becomes si or -s (byl si, kdes byl). This matches the [pronunciation guide](../../reference/suno/pronunciation-guide.md#czech-pronunciation).
- **Never rhyme only on obecná endings** (-ej, -aj, -ama). That is grade D.
- **No literary or archaic words** unless the song wants that irony: neboť, jenž, nechť, zřít, pravím, ó.

### Which Register When

**The artist's register rule comes first.** Check `{overrides}/CLAUDE.md` (and the album README) before choosing. If the user has set a register, it overrides the defaults below for every line, including rhyme words. Never reach for an obecná -ej form to complete a rhyme when the artist writes in spisovná. Common user rules:
- **Spisovná + explicit**: standard forms (dobrý, být, mléko, jsem) with vulgarisms allowed. A common choice for Moravian and Silesian artists, who don't use the Bohemian -ej forms. Rhyme pools shrink (no -ej family), so lean on stems, multis and assonance.
- **Obecná**: the Bohemian street default in the table below.
- **Regional colour**: a few regional markers as accent only. Ask which words are welcome and which read as cliché.

With no user rule set, use this table:

| Style | Register |
|-------|----------|
| Street rap, trap, drill | Obecná, consistently |
| Conscious or storytelling | Neutral or lightly colloquial. Gravity without stiffness; no literary words |
| Melodic or pop rap | Neutral colloquial, light slang, singable vowels |
| Comedy or irony | A deliberate clash of registers, flagged in the track concept |

### Regional Voices

Obecná čeština is Bohemian. Moravian and Silesian speakers often keep standard ý and é and have their own regional features; Ostrava-region speech is known for short vowels.
- Don't put Bohemian -ej forms into a persona from Brno or Ostrava unless the user asks for it.
- If the album has a regional identity, ask before writing.

### Slang and Anglicisms

Keep it to one strong slang word per line, and make sure it fits the persona's age and city. Rhyme loans by their Czech pronunciation.

| Word | Meaning | Inflection |
|------|---------|------------|
| prachy | cash | Plural only: prachy, prachů, s prachama |
| lóve | cash (from Romani) | Indeclinable |
| keš | cash | Use mostly in the nominative and accusative (mám keš) |
| litr / meloun | 1,000 Kč / a million | Hard masculine |
| brácha | bro | Declines like předseda: vocative brácho, instrumental bráchou |
| bro | bro | Indeclinable |
| týpek | guy | Genitive týpka; plural týpci |
| kámo / kámoš | mate | Vocative kámo; plural kámoši |
| beat | beat | Hard masculine: na beatu, beaty. Sung [bít] |
| flex / flexit / flexovat | flex | flexu; flexím; flexuju |
| drip | drip | dripu |
| hejtr | hater | Animate masculine: hejtra, hejtři |
| diss / dissovat | diss | dissu; dissuju |
| čilovat | chill | čiluju. The Czech spelling avoids the risky ch |
| postnout / lajknout | post / like | Perfective -nout: postnu, lajknu |
| money, party, Gucci | — | Indeclinable (they end in a vowel) |

**Patterns**:
- English nouns ending in a consonant decline like hard masculines.
- English verbs take -ovat (imperfective), -it, or -nout (a one-off action).
- English words ending in a vowel stay indeclinable.

### Spelling: Suno vs Streaming

- **Suno lyrics**: full diacritics, colloquial forms as sung, and slang in Czech spelling (keš, čil, hajp, flou, okej). See the slang table in the [pronunciation guide](../../reference/suno/pronunciation-guide.md#czech-pronunciation).
- **Streaming lyrics**: what is sung, in normal Czech orthography. Colloquial forms stay colloquial (dobrej). Respellings made only for Suno (lež → leš) revert, as with every respelling in this plugin.

---

## Common Failure Modes of AI-Written Czech Lyrics

**1. Forced inversion**
- **What happens**: the adjective or possessive is moved behind its noun to land a rhyme. It sounds like 19th-century poetry.
- **Examples**:
  - ❌ "Ten svět krutý mě nezlomí" → ✅ "Tenhle krutej svět mě nezlomí"
  - ❌ "Srdce mé už nebije" → ✅ "Srdce už mi nebije"
- **Fix**: rewrite the line around a new rhyme. Never reorder words to keep the old one.

**2. Calques from English**
- **What happens**: an English idiom is translated word for word. Czech has its own idiom, or none.
- **Examples**:
  - ❌ "To dělá smysl" → ✅ "To dává smysl"
  - ❌ "Mám tvoje záda" → ✅ "Kryju ti záda"
  - ❌ "Na konci dne je to jedno" → ✅ "Nakonec je to stejně jedno"
  - ❌ "Jsem v tom pro prachy" → ✅ "Jde mi jen o prachy"
  - ❌ "Žiju svůj nejlepší život" → ✅ "Užívám si naplno"

**3. Wrong case, gender or number agreement**
- **What happens**: Czech grammar is checked as loosely as English.
- **Examples**:
  - ❌ "Viděl jsem tvoje sestra" → ✅ "Viděl jsem tvoji sestru"
  - ❌ "Celý noc" → ✅ "Celou noc"
  - ❌ "Dva auta" → ✅ "Dvě auta"
  - ❌ "Pět kluci" → ✅ "Pět kluků"
  - ❌ "S moji holkou" → ✅ "S mojí holkou" (here the length of í is grammar)
- **Narrator gender**: past-tense and adjective forms encode the narrator's gender. A female narrator says "Byla jsem sama", never "Byl jsem sama". Match the vocal gender in the Style Box.

**4. Wrong verbal aspect**
- **What happens**: the perfective is used where the imperfective is needed. Ongoing or general activity needs the imperfective, and a perfective present means the future.
- **Examples**:
  - ❌ "Začal jsem napsat sloku" → ✅ "Začal jsem psát sloku" (začít and přestat take only the imperfective infinitive)
  - ❌ "Teď napíšu sloku", meaning "I'm writing a verse now" → ✅ "Teď píšu sloku". (The ❌ version means "Now I'll write a verse".)
- **Not an error**: the perfective present in habitual contexts means one completed act each time ("Vždycky přijde pozdě"). Don't "correct" it.

**5. Grammatical rhymes (gramatické rýmy)**
- **What happens**: the rhyme comes from matching endings, which Czech hands out for free.
- **Example**:
  ```
  ❌ Nechci ti nic slibovat,
     chci jenom tvrdě pracovat.            (-ovat – -ovat, grade D)

  ✅ Sliby nechám jiným, já mám vlastní plán,    (11)
     nikdo mi nešéfuje, jsem sám sobě pán.      (12)   (plán – pán, B)
  ```
- **Fix**: change the end word's word class. Infinitives and verbal nouns at line ends are the usual culprits.

**6. Filler words**
- **What happens**: prostě, jako, fakt, teda, vlastně, furt or a line-final vole or jo pads the syllable count.
- **Example**: ❌ "Sem prostě fakt jako unavenej, vole" → ✅ "Sem unavenej, klížej se mi oči"
- **Fix**: use the freed syllables for an image. Ad-libs go in parentheses.

**7. Rhyme-driven nonsense**
- **What happens**: the rhyme word is chosen first and the meaning bent to fit.
- **Example**:
  ```
  ❌ Jedu městem jako drak,
     v kapse mám jen starej mrak.          (a cloud in my pocket means nothing)

  ✅ Jedu nočním městem, nad hlavou mrak,       (10)
     poslední stovku dám za první vlak.         (10)   (mrak – vlak, B)
  ```

**8. Cringe rapper clichés**
- **What happens**: stock boasts stand in for detail.
- **Examples**:
  - ❌ "Šel jsem z ulice až na vrchol"
  - ❌ "Hejtři mě nezastaví"
  - ❌ "Vstávám jak fénix z popela"
  - ❌ "Sem král týhle hry"
  - ✅ "Dřív jsem vracel flašky, abych měl na tramvaj". A concrete detail proves the come-up; a claimed status doesn't.

**9. Overlong lines**
- **What happens**: a line carries a whole paragraph. Suno rushes it and swallows the consonants.
- **Example**: ❌ "Ráno vstávám do práce a celej den makám, ale večer zase nemám nic" (22 syllables) → ✅ "Celej den makám, večer zase nic" (10)

**10. Clitics out of second position**
- **Examples**:
  - ❌ "Co dal jsem ti, to vrátíš" → ✅ "Co jsem ti dal, to vrátíš"
  - ❌ "Se mi to nelíbí" in a standard or neutral verse → ✅ "To se mi nelíbí" (in obecná street register the ❌ form is real speech; use it only as a deliberate persona marker)
  - ❌ "Koupil jsem to si" → ✅ "Koupil jsem si to"

**11. Wrong syllable on the beat**
- **What happens**: a non-initial syllable lands on the snare (u-LI-ce, ka-MA-rád, pe-NÍ-ze).
- **Fix**: shift the line so the word's first syllable takes the snare, as in [Worked Fixes](#worked-fixes), or swap the word.

**12. Register mixing and literary words**
- **Examples**:
  - ❌ "Sem unavenej a nemohu spát" → ✅ "Sem unavenej a nemůžu spát"
  - ❌ "Neboť jsem zřel tvou tvář" → ✅ "Protože jsem tě viděl"

**13. English drifting into a Czech line**
- **Example**: ❌ "Jedu městem, baby, I'm on my way" → ✅ "Jedu městem, jsem na cestě". Or give the English its own `[Hook]` section.

---

## Explicit Content

The base word list in `check_explicit_content` (`handlers/text_analysis.py`) is English-only, so Czech profanity is not detected.
- **Set the Explicit field yourself** for Czech lyrics.
- **Or register the words** in `{overrides}/explicit-words.md` under `## Additional Explicit Words`, one `- word` bullet per form.
  - Matching is whole-word and case-insensitive.
  - Czech inflects, so list every form you actually use (for example zmrd, zmrdi, zmrdů).

---

## Per-Bar QA Checklist

Run this on every Czech verse and hook, line by line, before presenting. Count and mark in your working notes; the CAPS and counts never go into the Suno Lyrics Box.

**Q1 Syllables**
- Count by hand with the Czech rules.
- Rhyming partners stay within ±2.
- Each line falls inside the band for the delivery ([Bar Density by Tempo](#bar-density-by-tempo)).

**Q2 Stress groups**
- Mark the stressed syllables in CAPS.
- Group prepositions with their nouns.
- Attach enclitics to the preceding word.

**Q3 Beat placement**
- Every snare and hard accent carries a group-initial syllable, or the first syllable of a noun after an unstressed preposition.
- No non-initial syllable sits on a hard accent. A non-initial long vowel is allowed only on a held or sung note.
- Pickups are unstressed.

**Q4 Clitics**
- In second position, in the right order.
- No se/si, dative, accusative, conditional or past-auxiliary clitic starts a clause (copula jsem/sem excepted; clause-initial se/si only as a deliberate obecná persona marker).
- None carries a rhyme.

**Q5 End-rhyme grade**
- Grade every pair A/B/C/D/X with the [Grading Procedure](#grading-procedure).
- Check the grade against the [End-Rhyme Policy](#end-rhyme-policy).
- D or X means rewrite.
- Flag clichés like nebe – tebe.

**Q6 Internal rhyme**
- At least one internal rhyme or stress-aligned assonance link per couplet in rap verses.

**Q7 Grammar**
- Case, gender and number agreement.
- The case after numerals (dvě auta, pět kluků).
- Verbal aspect.

**Q8 Narrator**
- Past-tense and adjective gender (byl/byla, sám/sama, unavenej/unavená) is consistent and matches the vocal.
- POV is consistent.

**Q9 Naturalness**
- Would a native speaker say this sentence?
- No inversion, no calques, no rhyme-driven nonsense.

**Q10 Register**
- One register throughout.
- Spelled as sung.
- No literary words unless deliberate.

**Q11 Filler and clichés**
- No padding words.
- No stock rapper clichés.

**Q12 Clusters and tempo**
- Read the line aloud at tempo.
- Heavy clusters stay out of fast passages and triplets.

**Q13 Suno hygiene**
- Diacritics intact.
- Numbers and abbreviations written as Czech words.
- Slang in Czech spelling.
- English only in its own section.
- No CAPS or extra accent marks.

### Where Each Check Plugs into the 13-Point Check

| 13-point item | Czech addendum |
|---------------|----------------|
| 1. Rhyme check | Q5. Grammatical (D) and identical (X) rhymes are the Czech "lazy patterns" |
| 2. Prosody check | Q2, Q3, Q4 |
| 3. Pronunciation check | Q13, plus the [Czech Pronunciation](../../reference/suno/pronunciation-guide.md#czech-pronunciation) risks (ř, ch, c, English-looking words). English lines still go through `check_homographs` |
| 4. POV/Tense check | Q8, plus aspect from Q7 |
| 7. Flow check | Q1, Q9, Q11, Q12 |
| 8. Length check | Use the Czech word band ([Word Count](#word-count)) |
| 10. Rhyme scheme check | Q5, Q6. AABB couplets by default; no orphan lines |
| 11. Density/pacing check | Q1 against the density table and the genre README line |
| 13. Pitfalls check | Q7, Q9, Q10, Q11, plus [Common Failure Modes](#common-failure-modes-of-ai-written-czech-lyrics) |
| 5, 6, 9, 12 | Unchanged |

**Reporting**: report each violation under its 13-point number, with the Q code and a fix. For example:
- "#1 / Q5 — V1 L4: dělat – volat is grade D (infinitive ending). Proposed: …"
- "#2 / Q3 — V2 L3: u-LI-ce lands on the snare. Start the line two slots later: …"

---

## Worked Example: 8-Bar Verse

**Brief**: an original verse. Half-time trap at 140 BPM (felt 70), rapped in straight 16ths. AABB, obecná čeština, male narrator. Two topics: the night-shift grind (with a message from his mother) and the stage as the way out.

### As It Goes into the Suno Lyrics Box

```
[Verse 1]
Zima jak prase, v kapse nová zpráva,
na skladě zase jenom horká káva.
Máma píše, ať už jedu zpátky,
že prej nemá cenu žít na splátky.
Tahám palety, bolí celý tělo,
před lety sem žil, jak se mi chtělo.
Ruce černý od prachu, pořád nemám prachy,
ale na scéně už neumírám strachy.
```

The verse keeps its diacritics and uses no digits, no CAPS and no English. "sem" is the obecná spelling of jsem, consistent with prej, celý tělo and černý.

### On the Grid

Each line is one felt bar of 16 slots at felt 70 BPM. Kick on beat 1, snare on beats 2 and 4.

```
slot   1     e     &     a     2     e     &     a     3     e     &     a     4     e     &     a
drums  K                       S                       K                       S
L1     ZI    ma    jak   ·     PRA   se    KAP   se    NO    vá    ·     ·     ZPRÁ  ~     va    ·
L2     NA    skla  dě    ·     ZA    se    JE    nom   HOR   ká    ·     ·     KÁ    ~     va    ·
L3     MÁ    ma    ·     ·     PÍ    še    AŤ    už    JE    du    ·     ·     ZPÁT  ~     ky    ·
L4     ·     ·     že    prej  NE    má    CE    nu    ŽÍT   ~     ·     na    SPLÁT ~     ky    ·
L5     TA    hám   ·     ·     PA    le    ty    ·     BO    lí    CE    lý    TĚ    ~     lo    ·
L6     PŘED  le    ty    sem   ŽIL   ·     ·     ·     JAK   se    mi    ·     CHTĚ  ~     lo    ·
L7     RU    ce    ČER   ný    OD    pra   chu   ·     PO    řád   NE    mám   PRA   ~     chy   ·
L8     A     le    ·     na    SCÉ   ně    už    ·     NE    u     mí    rám   STRA  ~     chy   ·
```

**Beats**:
- Every beat carries a stressed syllable, except beat 1 of L4, which is a rest before the pickup "že prej".
- SPLÁT (L4) and SCÉ (L8) take the snare after the unstressed pickup "na" (beat rule 5).
- No non-initial syllable sits on any beat.
- ŽIL (L6) is followed by rests, not a three-slot hold: a long hold on a short vowel makes it sound long (žííl). Hold only long vowels ([Melodic Trap and Held Notes](#melodic-trap-and-held-notes)).

**Rhymes**:
- **End rhymes**: all on beat 4.
- **Internal echoes**: PRA-se / ZA-se share beat 2 in L1–L2. PA-le-ty (L5, beat 2) ladders into PŘED le-ty (L6, beat 1).
- **The closing multi**: "mám PRA-chy" and "rám STRA-chy" occupy identical slots (12–15) in L7–L8.

### Annotation

| # | Stress (CAPS) | Syll. | End rhyme | Grade | Notes |
|---|---------------|-------|-----------|-------|-------|
| 1 | ZI-ma jak PRA-se, v KAP-se NO-vá ZPRÁ-va | 11 | nová zpráva | A | Internal chain: prase, kapse |
| 2 | NA skla-dě ZA-se JE-nom HOR-ká KÁ-va | 11 | horká káva | A1 with L1: O-á-Á-a, stress-aligned, clean [áva] | prase – zase is a clean B on beat 2 in both lines |
| 3 | MÁ-ma PÍ-še, AŤ už JE-du ZPÁT-ky | 10 | jedu zpátky | B | "už" is an unstressed unstable enclitic here |
| 4 | že prej NE-má CE-nu ŽÍT na SPLÁT-ky | 10 | na splátky | B with L3: [átki]; na is a pickup (beat rule 5) | "že prej" is the pickup. jedu – cenu is an e-u assonance link (C, internal) |
| 5 | TA-hám PA-le-ty, BO-lí CE-lý TĚ-lo | 11 | celý tělo | A | |
| 6 | PŘED le-ty sem ŽIL, JAK se mi CHTĚ-lo | 10 | se mi chtělo | A2 with L5: supporting ť ([ťelo]); noun vs verb | Ladder: palety → před lety (A2). sem follows "před lety"; se mi follows "jak" |
| 7 | RU-ce ČER-ný OD pra-chu, PO-řád NE-mám PRA-chy | 13 | nemám prachy | A | Deliberate pun: od prachu (dust) vs prachy (cash), internal, not graded |
| 8 | A-le na SCÉ-ně už NE-u-mí-rám STRA-chy | 12 | neumírám strachy | A1 + A2 with L7: unstressed á, stressed a, unstressed i, plus the supporting r | na is a pickup before SCÉ (beat rule 5). neumírám = ne-u-mí-rám, 4 syllables |

**Totals and checks**:
- **Syllables**: 88 across 8 lines, 10–13 per line, inside the 10–14 band for rapped trap. Partner differences are 0, 0, 1 and 1 (all within ±2).
- **Words**: 52.
- **Rhyme map**: AABB. The end rhymes run A, B, A, A. The single B couplet is clean, and the build to A in the last two couplets gives the verse its lift.

### QA Run

| Check | Result |
|-------|--------|
| Q1 | ✅ 11/11, 10/10, 11/10, 13/12 |
| Q2–Q3 | ✅ See the grid. Every snare carries a group-initial syllable, or the first syllable of a noun after an unstressed preposition (SPLÁT, SCÉ). No u-LI-ce errors |
| Q4 | ✅ "sem" and "se mi" sit in second position. No clause starts with a se/si, dative, accusative, conditional or auxiliary clitic. No line ends on a clitic |
| Q5 | ✅ No D or X. A/B only at line ends |
| Q6 | ✅ Every couplet has a link: prase/kapse/zase; jedu/cenu; palety/před lety; prachu/prachy |
| Q7–Q8 | ✅ celý tělo and ruce černý are consistent obecná agreement. The male narrator is consistent (žil). The ongoing grind is imperfective (tahám) |
| Q9–Q11 | ✅ Natural word order, no calques, no filler. Concrete detail (pallets, warehouse coffee, installments, dusty hands) instead of status claims |
| Q12 | ✅ No heavy clusters (no vzp-, čtvr-, zmrzl-). The light ones (skl-, sc-) sit in 11- and 12-syllable lines with rests |
| Q13 | ✅ Diacritics intact, no digits, no English, no CAPS |

---

## Sources

- [Skarnitzl 2014 — prepositions and stress groups in Czech](https://fonetika.ff.cuni.cz/wp-content/uploads/sites/104/2015/10/Ska14-predlozky.pdf). Covers stress-group boundaries (|proti |vnějším vs |protivnějším, after Palková), preposition stress (68% of cases on the preposition in read news, 76% in spontaneous speech; the shift to the next word grows with its length and evens out the rhythm; Zeman 1980 data), Czech as fixed stress that ignores vowel length, and weak acoustic stress.
- [CzechEncy — Přízvuk](https://www.czechency.org/slovnik/P%C5%98%C3%8DZVUK). Fixed initial stress; vowel length is not a stress cue; the delimitative function is described as potential and often not signalled acoustically.
- [Kosek 2016 — enclitics in Czech (Bohemica Olomucensia)](https://bohemica.upol.cz/pdfs/boh/2016/03/06.pdf). Stable and unstable enclitics.
- [cs.wikipedia — Rým](https://cs.wikipedia.org/wiki/R%C3%BDm). The two-syllable norm; bohatý and dobrý rhymes; asonance.
- [Sgallová 2015, *O českém verši* (Karolinum), book preview](https://core.palmknihy.cz/api/books/331939/preview.pdf). Refines Hrabák's definition of grammatical rhyme into first and second degree (Hrabák 1958 had classed chodíme – vodíme as split rhyme); the supporting consonant (*opěrná souhláska*); line counts from Rubeš's declamatory verse.
- [Malý anglicko-slovenský slovník verzologických pojmov](https://unibook.upjs.sk/img/cms/2023/ff/maly-angl-slov-slovnik-verzologickych-pojmov.pdf). Masculine and feminine rhyme; mosaic rhyme.
- [elon.io — obecná čeština features](https://elon.io/grammar/czech/register/obecna-cestina-features).
- [Czech RapCor Boosted v1 (RASLAN 2025)](https://nlp.fi.muni.cz/raslan/2025/paper18.pdf). A corpus of 7,211 Czech rap songs, dominated by colloquial forms.
- [Duinker 2019 — Good Things Come in Threes: Triplet Flow in Recent Hip-Hop Music](https://www.cambridge.org/core/journals/popular-music/article/good-things-come-in-threes-triplet-flow-in-recent-hiphop-music/99BC46987A0BF369A0A3CCFC54F1CDBB).
- [Chodaková 2016 — rhythm and stress in Czech and French rap (dissertation)](https://dspace.cuni.cz/handle/20.500.11956/82400). The most relevant academic study. Its full findings were not reviewed for this file.

Rules marked "practitioner rule" or "heuristic" (the long-vowel held-note rule, the secondary stress in long words, the density bands, the stress-alignment downgrade, the word-count band) are craft conventions, not findings from those sources.
