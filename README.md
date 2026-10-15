# Song lyrics corpus — public release

Thirty-four song-lyric texts in English, Spanish, Catalan, Japanese, Mandarin
Chinese and Arabic, with one bilingual English/Spanish duet. They were
assembled as the standard test-song corpus for a set of language-learning
tools. Each text is public domain or carries a licence that allows commercial
use, educational use and redistribution. Each has a rights record that states
its basis, the evidence for it, and where else it is clear. The documentation
is CC BY 4.0; "Licensing in brief" below gives every file's terms.

This repository holds texts and their records only, with no software, audio
or music. It is released from the United States. The corpus is a subset of a
corpus used for private development in the United States.

## Contents

- `songs/` — one slug per song, flat and 0-indexed; the numbering is not
  contiguous:
  - `song_<n>.txt` — the lyric text, UTF-8. For the Chinese songs it is the
    simplified-character edition.
  - `song_<n>.rights.md` — the song's rights record (format below).
  - `song_<n>.zh-hant.txt` (song_13–18) — the traditional-character source
    edition, verbatim. The `.txt` beside it is a recorded OpenCC conversion of
    it, and any residual glyphs are listed in the record's `edition:` field.
  - `song_<n>.translit.txt` (song_26, song_27) — the verbatim pre-1929
    Latin transliteration that the song's Arabic file renders. It is a witness,
    not a separate song.
- [`RIGHTS_LEDGER.md`](RIGHTS_LEDGER.md) — one row per song, with its rights
  basis, tier and release status.
- [`NOTICE.md`](NOTICE.md) — attribution, licence notices, and the
  jurisdiction notes a reuser should know.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — how a song is proposed: the
  search strategy, the rights gate, the text and record conventions, and the
  lessons learned while the corpus was built. Acceptance stays with the
  maintainer.
- [`LICENSE`](LICENSE), [`REUSE.toml`](REUSE.toml) and `LICENSES/` — the
  terms, and the machine-readable status of every file
  ([REUSE](https://reuse.software/) format).
- `.gitattributes` turns off all line-ending conversion, so the texts stay
  byte-for-byte as recorded.
- [`CITATION.cff`](CITATION.cff) — citation details, if you want to cite the
  corpus (GitHub shows them as "Cite this repository"); citing is optional.

**Composition (34):** English 5 (song_0, 1, 10, 29, 30); Spanish 3 (song_4
Mexican, song_5 Cuban, song_12 Argentine) and Catalan 1 (song_3); Japanese 8
(song_6, 8, 9, 11, 32–35); Mandarin Chinese 6 (song_13–18); Arabic 10
(song_19–28: Modern Standard, Classical, and the Egyptian, Moroccan, Kuwaiti
and Palestinian dialects); bilingual English/Spanish 1 (song_31). The slug does
not tell you the language: the ledger and the record do.

## The standard

### Admission gate

A song's **lyrics** must be public domain in the United States **and** in the
country of origin, or carry a licence that allows commercial and educational
use and redistribution. CC BY-SA is acceptable; NC, ND and research-only
licences are not. "Public domain in the US" alone, or "public domain at home"
alone, does not qualify. Only the lyrics are assessed and shipped. A song also
has a composition and recordings, with rights of their own, and none of those
is here.

### Jurisdiction tiers

Public-domain status is decided country by country. The gate covers two
countries. Elsewhere, a foreign song's status depends on the country's own
term and on whether it applies Berne's **rule of the shorter term** (the
comparison of terms), under which a foreign work is protected no longer than
at home. A country that applies the rule follows the source country. A country
that does not apply it protects the song for its own full term. So a song can
be public domain at home and in the US and still be protected there.

**Reference groups** (checked 2026-09-29 against the Wikipedia tables "Rule
of the shorter term" and "List of countries' copyright lengths" and the
Wikimedia Commons page "Copyright rules by territory"; re-checked on
2026-10-14, when none of the three pages had been edited since):

| Group | Countries | Term |
|---|---|---|
| Longest tail, no comparison of terms | Mexico | life+100; the extensions never revived expired works, so authors dead before 1952 are clear |
| | Colombia; Equatorial Guinea | life+80 |
| | Jamaica | life+95 for authors dead from 1962 on; life+50 before that |
| | St Vincent and the Grenadines | life+75 |
| Life+70, no comparison of terms | Australia (authors dead before 1955 stay clear), Brazil, Switzerland, Indonesia, Turkey, Iceland, Nigeria, Paraguay, Côte d'Ivoire (life+70 since 2016), Canada (authors dead before 1972 stay clear) | life+70 |
| EU special cases | Spain: life+80 for authors who died before 7 December 1987 (an acquired right; binds EU-national lyricists, and third-country lyricists only if their home term is itself 80 or longer). France: wartime extensions, plus 30 years for authors "mort pour la France", surviving only where the pre-1995 total already exceeded life+70 — up to life+94 years 272 days; EU-national lyricists only. Germany: no comparison of terms for US-origin works (1892 US–German treaty), so a US work gets the full German life+70 | longer than 70 in the stated cases |
| Applies the comparison of terms | EU/EEA and UK, Japan, South Korea, India, Russia, Israel, Norway, Argentina, Singapore, Thailand, Taiwan, Hong Kong, Macau, Guatemala, Honduras, and most others | follows the source country |
| Life+50 or shorter | New Zealand, Philippines, South Africa, Malaysia, Vietnam, Lebanon, Nepal; the source countries China, Egypt, Tunisia, etc. | never binds a song that is public domain at home |
| United States | | fixed dates: first published before 1931 is public domain (the bound rises each January); a URAA-restored work gets at most 95 years from publication |

In the EU (Directive 2006/116/EC), the comparison of terms is mandatory for a
work from a third country by an author who is not an EU national, so every
lyricist in this release gets at most the home term anywhere in the EU. Older
treaties prevail, which gives the Germany–US exception above.

**The tiers** turn on one verifiable fact: the lyricist's death year, or the
song's anonymity, measured against the current year. They are recomputed each
January. A song can only rise (Tier 2 → 1 → 0); it falls only if the
reference tables change.

| Tier | Test (bounds as of 2026) | Clear where | Exposure remaining | Allowed use |
|---|---|---|---|---|
| **Tier 0 — universal** | anonymous or traditional; or the lyricist died before **1946** (the bound is the earlier of "current year − 80" and 1952; from 2053 it is "current year − 100") | every country under every known term rule | none known | any use, including public release |
| **Tier 1 — life+70 has run** | lyricist died before **1956** but not Tier 0 | US, country of origin, every comparison-of-terms country, every life+70-or-shorter country | Colombia and Equatorial Guinea to death+80; St Vincent and the Grenadines to death+75; Mexico to death+100 | excluded from public release until it reaches Tier 0 |
| **Tier 2 — US and origin only** | public domain in the US and the country of origin, but the lyricist died **1956 or later** | US, country of origin, every comparison-of-terms country (for a US-origin work, all but Germany), every life+50 country | as Tier 1, plus Jamaica to death+95 for lyricists dead from 1962, and the life+70 countries that do not compare terms, to death+70 | excluded from public release |
| **Tier L — licensed** | CC0, CC BY or CC BY-SA, or an author's or rights holder's public-domain dedication or grant (never NC, ND or research-only) | worldwide, by the licence or grant | attribution and, for CC BY-SA, share-alike, which rides on derived artefacts | any use, with the obligations carried |

Notes (the records cite these as "README, 'Jurisdiction tiers', notes"):

- **EU-national lyricists:** Spain's life+80 sits inside the Tier 0 bound;
  for a lyricist "mort pour la France", Tier 0 needs "died before current
  year − 95". Third-country lyricists need neither check.
- **Folklore regimes are not copyright terms.** Several Arab states (for
  example Jordan, Egypt and Morocco) vest never-expiring, state-held
  exploitation rights in national folklore. Mexico's regime (Ley Federal del Derecho
  de Autor, Arts. 157–160, as reformed on 2020-01-24) requires the written
  authorisation of the people or community that holds a traditional cultural
  expression before it is exploited. These regimes bear on commercial use
  inside those states, and the tiers do not model them. The records of the
  songs concerned note them, and [`NOTICE.md`](NOTICE.md) states them.
- **A project-made Arabic rendering of a transliterated witness** (song_26,
  song_27) does not change the rights analysis. The song is anonymous, the
  witness adds no authored layer of the collector's, and the rendering is a
  conversion. It is not a published Arabic text, though: the verbatim
  transliteration is kept beside it as `song_<n>.translit.txt`, and the record
  marks the Arabic file as a rendering.
- **Tier L** records rest on a dedication or a licence rather than a death
  year. song_29–31 (the author's dedication) and song_34–35 (the rights
  holder's grant) cite the grant in `tier_basis`, and their records note how
  the express permission operates in jurisdictions that do not recognise
  abandonment of copyright. song_32–33 (CC BY-SA 4.0)
  record the share-alike condition, which rides on any adapted artefact that
  includes their text.
- **Moral rights** (attribution, integrity) are perpetual in several
  countries. Every record names the lyricist and the source edition. A text is
  either verbatim from its cited source, or its record's `edition:` field
  lists every departure, and any character-set conversion is labelled.
- **Derived artefacts inherit the tier of their song** when the text can be
  recovered from them: token-level parses with surface forms, line tables,
  screenshots, documents quoting lines. Aggregates that reproduce no text
  (counts, grades, offsets without text, hashes) carry no exposure.
- **"Pre-1929" in the records and the ledger** is the US publication bound as
  it stood when the records were first written. The bound rises each January
  and is 1931 in 2026, so every such statement remains a sufficient condition.

## Tier snapshot for this release

As of 2026-10-14, against the reference groups above:

| Tier | Songs | Slugs |
|---|---|---|
| 0 — universal | 27 | song_0, 1, 3, 4, 5, 6, 8, 9, 10, 11, 12, 13–28 |
| L — licensed or dedicated | 7 | song_29–31 (author's dedication), song_32–33 (CC BY-SA 4.0), song_34–35 (rights holder's grant) |

Tier 0 does not fall unless the reference tables change, and Tier L does not
move. Each later release re-tiers first.

## The rights records

Each `songs/song_<n>.rights.md` records at least:

```
title:            the song title
author/lyricist:  the LYRICS author with birth–death dates, not the performer
composer:         the music's author (the music is not included)
language:         en | es | ca | ja | zh | ar | en+es
genre:            genre, to show the set's diversity
register:         (ar, zh) classical | literary | vernacular | dialect
edition:          the pinned source state: the revision or scan page read and
                  when, line and stanza counts, every normalisation and
                  exclusion, and differences from any dated witness
rights_basis:     public-domain | the exact licence id (e.g. CC-BY-SA-4.0)
allowed_uses:     commercial, educational, redistribution
jurisdiction:     where the status was verified
tier:             0 | 1 | 2 | L, and the date it was assigned
tier_basis:       the fact the tier rests on
residual_exposure: none | each country where the lyrics are still protected
tier_changes:     when the song rises a tier
release:          what the tier allows ("public release eligible" here)
evidence:         the basis and the sources that prove it
sources:          links
verified_by:      the person who made the rights call
verified_on:      YYYY-MM-DD
notes:            caveats, history, the values screen
```

**The records are good-faith determinations, not legal advice.** A person,
the developer, made each rights call. Automated research assisted, and the
records say where Claude Code drafted a passage. Each record keeps its
evidence trail so you can check it yourself. Laws and terms differ by
country. If you need certainty for a particular use, take your own advice.

Where a record refers to "the README", it means this file: the admission
gate, "Jurisdiction tiers", the "Tier L" note above, and the release process
below. Where a record addresses "the reviewer", it means the developer at
acceptance: a "may check" or "should check" sentence records a cross-check
that was offered when the record was drafted, and the record's DEVELOPER
REVIEW and DECISION entries record what was done. "Staged" in a record means
placed in the song's text file.

The records are plain-text layouts. GitHub's rendered view runs their fields
together, so read them in its Code view or in an editor.

## The release process

Every release of this corpus follows the same steps. For this release:

1. **Release date and re-tier:** 2026-10-14; the snapshot is above.
2. **Release set by tier:** Tier 0 and Tier L only.
3. **Each song re-verified:** US and source-country status, source edition,
   lyricist and death year; `verified_on` updated 2026-10-14. Where a check
   rests on the earlier verification instead, the record says so (song_1,
   song_17, song_26 and song_27).
4. **Attribution and integrity:** the ledger and the records ship with the
   texts, and each text is verbatim or its departures are recorded.
5. **Licence obligations:** the licence texts, the attribution and the
   notices are in `LICENSES/`, `NOTICE.md` and `REUSE.toml`.
6. **No software:** this repository contains no software, and no corpus text
   ships inside software.
7. **Released from the United States** on GitHub, with the standard stated, a
   rights contact named, and the evidence trail kept in the records.
8. **Logged** in the "Releases" section of the ledger.

## Licensing in brief

Each text keeps its own status, and nothing in this repository adds a term to
it. The full terms are in [`LICENSE`](LICENSE), and the per-file status is in
[`REUSE.toml`](REUSE.toml).

| Files | Status |
|---|---|
| the 19 verbatim Tier 0 texts, and the song_13–18 `.zh-hant.txt` and song_26–27 `.translit.txt` witnesses | public domain; no rights claimed (`LicenseRef-PublicDomain`) |
| song_29–31 | the author's public-domain dedication (`LicenseRef-Lehrer-PD-Dedication`) |
| song_34–35 | the rights holder's public-domain grant (`LicenseRef-dotstokyo-PD-Grant`) |
| song_32–33 | CC BY-SA 4.0 alone; attribution and the licence notice are in `NOTICE.md` |
| the OpenCC editions (song_13–18 `.txt`) and the Arabic renderings (song_26–27 `.txt`) | the underlying text is public domain; the developer's conversion is waived under CC0 1.0 (`LicenseRef-PublicDomain AND CC0-1.0`) |
| the README, contributing guide, ledger, notice, records, `REUSE.toml`, `.gitattributes`, `CITATION.cff`, the `LICENSES/LicenseRef-*.txt` statements, and the selection and arrangement | CC BY 4.0, © 2026 shani; quotations in them keep their own status |

None of these terms restricts text and data mining or machine-learning
training. The texts are public domain, dedicated, granted or CC BY-SA, and
the developer's own material is CC BY 4.0, whose one condition is
attribution. GitHub shows the repository licence as "View license" because
the terms are composite; the per-file status is in [`REUSE.toml`](REUSE.toml).

## Rights questions and corrections

If you hold rights in a text here, or believe a determination is wrong, write
to shani, <shanigo@pm.me>. A text whose status is credibly questioned is
re-checked, and it is held out of the release if its determination cannot be
re-confirmed.

To propose a song, follow [`CONTRIBUTING.md`](CONTRIBUTING.md); a proposal
carries the record, the source pin and hashes, never the text itself.
