# Contributing: how a song enters this corpus

A runbook for proposing a song, written so that a person or an agent acting
for a person can follow it step by step, and a record of what was learned
while the corpus was built. A proposal that follows it arrives complete; the
maintainer still makes every rights call and decides what is accepted. Under
the terms in [`LICENSE`](LICENSE) you may also fork the corpus and extend
your fork on your own responsibility; the last section says what carries
over when you do.

Read first: [`README.md`](README.md) ("The standard", "Jurisdiction tiers",
"The rights records", "The release process"), [`RIGHTS_LEDGER.md`](RIGHTS_LEDGER.md)
for what is already in, and [`NOTICE.md`](NOTICE.md) for how the licensed and
granted texts are documented. This file adds the method; the README stays the
authority wherever the two differ.

## Hard stops

These end a proposal, or send it back a stage, whatever else is true of it.

1. **The proposer is never the authority for the rights call.** A proposal is
   a recommendation with evidence. The maintainer verifies it and decides.
2. **When in doubt, exclude.** If public-domain status in both the United
   States and the country of origin, or a qualifying licence, cannot be
   established with evidence, do not prepare a text file. Stop and report why.
3. **Tier 0 and Tier L only.** This corpus releases nothing that is still
   protected anywhere. A song that would land in Tier 1 or Tier 2 (README,
   "Jurisdiction tiers") is not accepted; report its tier, its residual
   exposure and the year it would reach Tier 0 instead of a text.
4. **No unverified lyric text in any public place.** Do not put the text in
   an issue, a comment, a public fork or a pull request, and do not quote
   lines in logs or transcripts. Prepare the files locally; the text enters
   this repository only when the maintainer accepts it (Stage 6). Refer to
   lines by number.
5. **Lyrics only.** A song also has a composition and recordings, each with
   rights of its own. Only the words are assessed and only the words ship.
6. **Values screen.** Songs that demean people or groups, glorify oppression
   or violence against people, or promote hatred are excluded whatever their
   rights status. An ambiguous case is excluded too; the corpus is small and
   needs no borderline text (Stage 1a).
7. **Verbatim, human-written text.** The file is the pinned source's text,
   with every departure recorded. Machine-generated or machine-translated
   lyrics, and local-language versions of a foreign song (the original author
   and the translator each hold rights), are out of scope.

## Inputs

Optional: a target language (`en`, `es`, `ja`, `zh`, `ar`; `ca` and `en+es`
exist as their own buckets), a rights class (public domain by age, or Tier L
by dedication, grant, CC BY or CC BY-SA), or a specific song to evaluate.
With no target, read the ledger's composition note and pick a gap: a region,
dialect, register, era or structure the language's set lacks. There is no
quota per language.

## Stage 0 — Rights-first triage (the search strategy)

The rights gate, not genre, kills most candidates. Lead with rights.

### Search these classes first, in this order

1. **Anonymous or traditional songs.** No author, so no life+N clock, and
   traditional works were not restored in the US by the URAA (below). Folk
   songs, carols, spirituals, work songs, children's rhymes, min'yō.
2. **Anything first published before the US cutoff.** As of 2026 that is a
   first printing before 1931; the bound rises by one year every January
   (works first published before "current year − 95"). The conservative
   form used in the records is "before 1929", because the URAA restored only
   works first published from 1929 on. Pair an early print with a long-dead
   author and the song clears everywhere.
3. **A named lyricist who died before the Tier 0 bound** (before 1946 in
   2026; README gives the moving rule). Fix the US status separately with a
   publication date or an anonymity finding.
4. **A rights holder's explicit release, or a verified CC BY / CC BY-SA
   licence (Tier L).** Rare, and the only route to modern text. Search for
   the *release act* first, then the text: Wikisource's PD-release and
   CC-Zero categories, Wikimedia Commons own-work song uploads with VRT
   permission tickets, a rights holder's own site. The corpus's examples are
   an author's dedication (song_29–31), a management's public-domain page
   (song_34–35) and Commons uploads with VRT tickets (song_32–33); see
   `NOTICE.md`. Found so far only for English and Japanese.

### Technique for a hard slot

- **Death-date first, not genre first.** For a constrained slot, list the
  lyricists of the target region and era who died early enough, then pick
  their best-fitting song. Searching by genre and checking rights afterwards
  burned the most effort.
- **Loosen in this order and stop at the first class that yields:**
  contemporary → mid-century → early twentieth century → traditional or
  pre-1929; Latin-script wish → loanwords → any clean regional song.
  "Contemporary" means Tier L; check the known veins and the dead ends below
  before a catalogue search.

### Known dead ends

- **Contemporary CC0 or CC lyrics found through music catalogues.** CC0
  music corpora are instrumental; most CC music is NC or ND, which
  disqualify; the Free Music Archive carries no lyric texts; Jamendo's site
  has no licence filter and its API needs a registered key; Bandcamp tag
  sweeps return instrumentals and NC releases; Japanese "free BGM" sites use
  custom terms that forbid redistribution; sites offering "CC0 lyrics" in
  bulk are machine-generated. What works is class 4 above.
- **A platform licence flag from an account that is not the lyricist's.**
  YouTube's CC BY option, SoundCloud's licence field and the Internet
  Archive's `licenseurl` are set by the uploader. They are evidence only when
  the account is the lyricist's, or their label's with the lyricist the same
  party, and only for text the licensor published. Pirated uploads carry CC
  flags too; a label's own storefront can contradict its platform flag.
- **"Copyable lyrics" and fan-transcription wikis** (Vocaloid, dōjin,
  general lyric wikis). The transcription being copyable does not license
  the words, which stay with the producer or circle.
- **Named-author twentieth-century songs whose lyricist died in 1956 or
  later.** Protected somewhere for decades; Tier 2 at best, so not accepted.
- **Adapted or translated foreign songs.** Double-encumbered.
- **Ambiguous authorship** on a death-date-critical call: sources disagree
  on who wrote the words, father versus son, original versus revival. You
  cannot run a life+N test on an unresolved author. Exclude.
- **Long national terms.** Mexico is life+100, Spain life+80 for authors
  who died before 1988, Colombia life+80. A named author from these
  countries needs the longer clock; prefer anonymous or traditional there.
- **Wikipedia's lists of CC-licensed albums.** Every vocal entry checked was
  NC, ND or not CC at all.

### The one rule that catches the subtle failures: the URAA

"Public domain in the source country" is not sufficient for the US. Under the
Uruguay Round Agreements Act, a *foreign* work had its US copyright
automatically **restored**, for 95 years from publication, if it was (a)
still protected in its source country on 1996-01-01 and (b) first published
in 1929 or later. A foreign song whose author died in, say, 1954 can be public
domain at home through life+70 and still be under US copyright. Escapes:
publication before 1929; a genuinely anonymous or traditional text; or a
publication so early that 95 years from it have passed.

**"Published" means printed copies of the words or score offered to the
public:** a songbook, sheet music, a magazine, a book. A sound recording made
before 1978 did not publish the song under US law (17 U.S.C. § 303(b)), so
"the 1928 record" is not a pre-1929 publication. Pin a dated print, or use a
route that needs none (anonymity, or public domain at home before
1996-01-01).

**Life+50 source countries** change the arithmetic: mainland China (also
Taiwan and Hong Kong), Egypt, Tunisia, Lebanon, Syria, Jordan, Iraq, Kuwait
(Morocco is longer; check each country), and **Japan for every author who
died before 1968**, because Japan's life+70 dates only from 2018-12-30 and
revived no expired work. With life+50, a lyricist who died in or before 1945
was public domain at home before 1996-01-01 and *nothing* was restored in the
US, whatever the publication year; this admits works of the 1930s and early
1940s by early-dead authors. A lyricist who died in 1946 or later, with a
1929-or-later publication, was restored for 95 years from publication. One
year of death date can flip the result. Anonymous works: 50 years from
publication. Write the reasoning into `evidence:`.

## Stage 1 — Discovery

Goal: one candidate that could fill a gap, found through the triage above.

1. Read the ledger and the README's composition to see what each language
   set already covers.
2. Draw from the source families that have worked (see "Where clearable
   texts were found" below): Wikisource per language, Wikimedia Commons and
   its per-language song categories, library scans on Commons and the
   Internet Archive, national-library image servers, the Library of
   Congress, and, for a contemporary slot, the Tier L veins of class 4.
3. Apply the selection priority: (1) rights, which is hard; (2) regional,
   dialect and register variety within the language, which proved the
   highest-value axis; (3) genre and era diversity within the language; (4)
   the values screen; (5) contemporariness as a tie-breaker among candidates
   that already clear, never a target to chase.
4. Record the candidate's identity: title, lyricist (the author of the
   words, not a performer), language and register, apparent genre and era,
   and the exact location of the text you will take.

## Stage 1a — Values screen

Read the candidate for its content and message, and consider its documented
historical meaning. Classify it **aligned** (affirms human dignity, liberty,
equality, the abolition of oppression), **neutral** (a love song, a children's
song, a work song: no values stance), or **contradicts** (hard stop 6).
Exclude a contradicting or ambiguous candidate and return to Stage 1. Write
the classification and a one-line reason into the record's `notes:`; the
maintainer confirms it. Surface your reasoning rather than asserting a
verdict.

## Stage 2 — Comparison to the existing corpus

Read the ledger rows, and the records, of every song in the same language.
Reject the candidate if it overlaps materially with one of them: the same
song or a variant of it, the same narrow genre, the same era and register, a
near-identical vocabulary profile. Otherwise write down *why* it is diverse
relative to the set (region, dialect, register, era, form); the maintainer
checks that claim.

## Stage 3 — Rights lookup (the gate)

Goal: establish, with evidence, that the **words** are public domain in the
United States and in the country of origin, or carry a qualifying licence or
grant, and that the song is Tier 0 or Tier L.

1. **Identify the lyricist and the dates:** the death year (for life+N
   countries) and the first publication year and print (for the US rule and
   as a fallback basis). Confirm the death year in at least two independent
   places (Wikidata, a national-library authority record, a dated obituary
   or biography).
2. **Public domain by age.** Confirm the source-country term and that it has
   run (life+70 in the UK and the EU; Japan life+50 for deaths before 1968;
   Mexico life+100; Spain life+80 for deaths before 1988; the life+50
   countries above). Confirm the US status: first printing before the cutoff,
   or anonymity, or the URAA analysis written out. Anonymous or communal
   authorship plus an old print clears both with no life+N clock.
3. **Licence or grant (Tier L).** Confirm the exact licence id, or the
   wording of the grant, and that it allows commercial use, educational use
   and redistribution. CC0, CC BY and CC BY-SA qualify; NC, ND and
   research-only clauses disqualify. The evidence standard, learned the hard
   way:
   - (a) the licence or grant must come from the lyricist, or from the party
     that holds the rights in the words; a co-written lyric needs every
     lyricist, or an assignee, behind it; a platform flag counts only when
     the account is the lyricist's or their label's;
   - (b) the text must be published by the licensor: a Commons file
     description, the rights holder's own page, the platform description. A
     video with on-screen lyrics is a text source of last resort;
   - (c) pin the grant: the Commons revision id and VRT ticket ids, or an
     archived capture of the page, compared with the live page;
   - (d) for a Japanese work, run a JASRAC J-WID negative check by title and
     by author name (著作者名), because a collecting-society registration
     would cut across a grant by the management;
   - (e) a "public domain" dedication by a living author or a company
     operates as an irrevocable, royalty-free licence where the law does not
     recognise abandonment (Japan, Germany, France); record it as such with
     the permission quoted verbatim;
   - (f) for CC BY-SA, record that share-alike rides on any adapted artefact
     that includes the text, and write the attribution string into
     `release:`.
4. **Two copyrights, and the opportunity in them.** A public-domain
   recording does not make the words public domain, and a later musical
   setting or arrangement does not block public-domain words. A song that is
   still protected can therefore yield a usable text if its words are an
   independently public-domain poem: take the poem from its own edition and
   cite that, not the song (song_5 is such a case: the poem's quatrains are
   in the corpus; the refrain the song is known by belongs to a lyricist who
   died in 1979 and is not).
5. **Assign the tier** from the README's table, and list the residual
   exposure and the dates the song would rise. For this corpus the result
   must be Tier 0 (anonymous, or died before the bound) or Tier L. Two
   checks beyond the table: an EU-national lyricist needs Spain's life+80
   (inside the Tier 0 bound) and, if "mort pour la France", a bound of
   "current year − 95"; a text taken from a modern critical edition may
   carry an edition layer protected in some EU states for up to 30 years
   from that edition (Directive 2006/116/EC, Art. 5; 25 years in Germany),
   so record the edition's date and whether, for an Arabic text, the
   vocalization is the first print's or the editor's.
6. **Regimes outside copyright.** Several states vest never-expiring rights
   in national folklore (Mexico's Ley Federal del Derecho de Autor, Arts.
   157–160, since 2020; Jordan's 1992 law, Art. 7; Egypt's 2002 law, Art.
   142; Morocco's 2000 law, Art. 7). They bear on commercial exploitation
   inside those states and do not change the tier; note them in the record
   for a traditional song from such a country, as the records of song_4 and
   song_26–27 do.
7. **Gate.** If the status cannot be established with evidence: STOP, no
   text file, report the candidate as rejected with the reason. If the status
   is established but the tier is 1 or 2: STOP, report the tier, the residual
   exposure and the rise dates. Do not stretch a weak rights call; a proposal
   that does is rejected.

## Stage 4 — The text file (prepared locally, not published)

Goal: the lyric file as it would ship, prepared where no one but you can read
it, so that the maintainer can re-derive it from your pin and compare.

1. **Naming.** The maintainer assigns the `song_<n>` slug at acceptance; the
   number is not part of the proposal. Use a working name locally.
2. **One pinned source, verbatim.** Take the text from the single source
   identified in Stage 3 and record exactly what you read: the Wikisource
   revision id, the Commons file and revision, the scan item and page or leaf
   numbers, and the date. Do not mix variants. Exclude the page's own
   furniture: headers, navigation, stanza numerals, footnotes, annotations,
   ruby glosses (note their removal).
3. **Extract programmatically and compare line by line.** Read the raw
   wikitext, the page's HTML, or the page image at full resolution; then
   check that every non-blank line of your file occurs, with whitespace
   collapsed, in the source text. Where the source is a transcription,
   compare again with a dated print. Six of the corpus's first thirteen
   texts turned out to be modern renderings of the prints their records
   cited; this check finds that in a minute. List every departure in
   `edition:`.

   ```python
   # containment check: every non-blank line of FILE occurs in SOURCE (text or
   # saved HTML with tags already stripped), whitespace collapsed
   import re, sys
   norm = lambda s: re.sub(r"\s+", " ", s).strip()
   src = norm(open(sys.argv[2], encoding="utf-8").read())
   for n, line in enumerate(open(sys.argv[1], encoding="utf-8"), 1):
       if line.strip() and norm(line) not in src:
           print(f"line {n} not found in source")   # prints the number only
   ```

   Where the pin is a page image, OCR it in memory and compare each line of
   your file with the OCR text, printing only line numbers and similarity
   ratios: the recognised text is the lyric, so hard stop 4 applies to it.
   Normalise both sides first (NFKD, casefold, letters and digits only, and
   drop accents and Arabic harakat, which OCR loses), and match each line
   against single OCR lines and adjacent pairs, since OCR splits and merges
   lines. On an old print a low ratio means "read this line in the image",
   not "wrong". Apple's Vision text recognition (accurate level, language
   correction off) read this corpus's Latin-script, Arabic and horizontal
   Chinese prints; it failed on a page of vertical Chinese type, where the
   check stays by eye.

4. **Layout conventions**, every one of them recorded in `edition:` when it
   involved a choice:
   - one lyric line per line; no leading whitespace; a blank line only where
     the source divides stanzas; a bracketed stage cue or a role label
     (`HE:` / `SHE:`) stays on its own line as the source has it;
   - UTF-8, LF line endings, a final newline, no trailing spaces; the
     record's line count must equal the file's;
   - native script exactly, no transliteration or normalisation; if the
     source is in an older orthography, keep it, or record the modern
     rendering you took and the print it departs from;
   - **Chinese:** `<name>.zh-hant.txt` is the verbatim traditional source
     edition and `<name>.txt` the simplified primary, produced by OpenCC
     `t2s` (the `opencc-python-reimplemented` package); list the residual
     pre-standard glyphs the conversion leaves. The MediaWiki zh-hans
     converter was not used because it maps 餘 to 馀;
   - **Arabic:** one hemistich per line; vocalization and kashida as the
     source has them, except that the line-filling kashidas of typeset
     sources are not reproduced; a print's Maghrebi letterforms are written
     as standard ق and ف and the record says so; section labels the print
     sets as lines stay as lines. A corpus rendering of a transliterated
     witness keeps the verbatim transliteration beside it as
     `<name>.translit.txt` and the record marks the Arabic file as a
     rendering (song_26–27);
   - **Japanese:** kana and kanji as the source has them; katakana loanwords
     and ASCII digits or quotes inside Japanese stay as written;
   - the record's `language:` line starts with the tag a reader will parse
     (`en`, `es`, `ja`, `zh`, `ar`; `en+es` for a bilingual text; `ca`),
     followed by the register in parentheses.
5. **Hashes.** Record each file's line count and SHA-256 for the proposal
   (`shasum -a 256 <file>` or `sha256sum <file>`). The maintainer re-derives the file from your
   pin and compares the hash; that is how the text is proposed without being
   published.

## Stage 5 — The rights record

Draft `<name>.rights.md` in the README's format ("The rights records"). The
first line is the header `# Rights record — <slug>`; use the working name and
the maintainer substitutes the slug. Then the fields, each as `field: value`
on its own line with continuation lines indented, in the README's order:

- `title`, `author/lyricist` with birth–death dates (the author of the
  words, not a performer; "Anonymous / traditional" with the collection
  history for a folk text), `composer` with dates and a note that the music
  is not included, `language` (tag first), `genre`, `register` where it
  helps (classical, literary, vernacular, dialect).
- `edition`: the pinned source state in full: revision id or scan page and
  the date read, line and stanza counts, every normalisation and exclusion,
  every difference from a dated witness, and for Chinese which character
  set is the primary text and that it is a conversion of the cited source.
- `rights_basis`: `public-domain`, or the exact licence id (`CC-BY-SA-4.0`),
  or `public-domain — RIGHTS-HOLDER DEDICATION/GRANT` with the grant quoted
  verbatim in the source language and translated.
- `allowed_uses`: `commercial, educational, redistribution`, all three.
- `jurisdiction`: the countries checked, naming the source country and the
  US and the rule applied in each.
- `tier`, `tier_basis`, `residual_exposure`, `tier_changes`, `release`: from
  the README's tier table; for this corpus `release` reads "public release
  eligible" and the tier is 0 or L. Write "worldwide" only when it is true
  and agrees with `residual_exposure`.
- `evidence` and `sources`: the links and the basis, written so the
  maintainer can check the call quickly: death year plus term, or
  publication year plus rule, or licence id plus permission ticket; the
  containment check's result; the witness comparison.
- `verified_by: PROPOSED-BY-<your name or your agent's name> (pending the
  maintainer's verification)` and `verified_on:` the draft date. Do not
  attest verification yourself; the maintainer replaces this line.
- `notes`: the values screen result and reason; the diversity argument;
  which text version this is and what it excludes; the music's status if it
  differs; folklore regimes; open questions.

Do not quote lyric lines in the record; refer to lines by number. The one
kind of quotation a record needs is a licence statement, grant or rights
notice, which is quoted verbatim with its source.

## Stage 6 — Submit the proposal

Open an issue in this repository, or write to the rights contact named in
the README, with the package below. The text file itself stays with you
until acceptance (hard stop 4).

```
Proposal: <working name>
Language: <tag> (<register>)
Gap it fills: <region / dialect / register / era / form>; nearest existing
  songs by slug and why this one differs
Lyricist: <name, birth–death> | Anonymous / traditional (<collection history>)
Composer: <name, dates> (music not included)
First publication: <print, place, year>; sound recordings noted but not relied on
Source pin: <URL + revision id | scan item + page or leaf>, read <date>
Rights basis and tier: <public domain by age | licence id | grant>; Tier <0|L>
US status: <rule applied, with the URAA analysis if the work is foreign and
  published 1929 or later>
Source-country status: <term, death year or anonymity, public domain since>
Residual exposure: none | <countries and dates>
Values screen: aligned | neutral; <one line>
Text: <n> lines, <m> stanzas, SHA-256 <hex>; departures from the pin: <list | none>
Companion files: <.zh-hant.txt | .translit.txt: lines, SHA-256> | none
Draft record: <the full .rights.md text>
Suggested REUSE line: <"Public domain, no rights claimed (Tier 0): <lyricist
  (dates)>, <print>." | the licence or grant id and attribution>
Uncertainties: <every open question, stated as a question>
```

What the maintainer does with it: retrieves the text from your pin,
re-derives the file by the Stage 4 conventions, compares the hash, verifies
the rights call and the tier, assigns the slug, replaces `verified_by` with
their own attestation (the record keeps who drafted it), adds the ledger row
and the REUSE annotation, writes the `NOTICE.md` entry for a Tier L text,
and includes the song in the next release, which re-tiers and re-verifies
the whole set first (README, "The release process"). A rejection comes with
the reason. A proposal with an open question is better than one with a guess.

## Checks before you submit

| Check | How | Pass condition |
|---|---|---|
| Rights-first triage applied | Stage 0 | the candidate is in class 1–4 and in no dead end |
| Values screen | Stage 1a | aligned or neutral, reason written |
| Diversity | Stage 2 | the record names the nearest songs and the difference |
| Gate | Stage 3 | US and source country both established with evidence; tier 0 or L |
| URAA | Stage 3 | written out for any foreign work first published 1929 or later |
| Tier L chain | Stage 3 | licensor holds the words' rights; text published by the licensor; grant pinned; J-WID negative for a Japanese work; share-alike noted |
| Text verbatim | Stage 4 | every non-blank line found in the pinned source, whitespace collapsed; every departure listed in `edition:` |
| Witness | Stage 4 | compared with a dated print where the pin is a transcription |
| File hygiene | `tail -c1 <file> \| od -c` shows `\n`; `grep -n '[[:space:]]$' <file>` prints nothing | final newline; no trailing whitespace; LF endings |
| Chinese pair | OpenCC `t2s` of the `.zh-hant.txt` equals the `.txt` | identical, residual glyphs listed |
| Record complete | every README field present; header line; language tag first; `tier`/`release` agree; line count equals the file's | no field missing; `verified_by` says PROPOSED-BY |
| No text in the open | the issue, the comments and your fork carry no lyric line | hashes and line numbers only |

## Where clearable texts were found

- **Wikisource, per language.** The best single source of pinnable
  public-domain text. Its licence templates encode the reasoning this
  runbook asks for: zh.Wikisource's `{{Pd|death|pub}}`, `{{Pd/1923|death}}`
  (published before 1929) and `{{Pd/1996|death}}` (expired at home before
  the URAA date); ja.Wikisource's Japan-PD and US-pre-1929 tags;
  en.Wikisource's `Category:PD-release` for author dedications. Caveats
  learned: a page's cited base text (底本) is not always what its text
  follows; a stub with no base text may be a modern rendering; a title can
  redirect to a different edition than the record names; a page's
  illustrations can be scans of a different print than its text; later
  pages of a long scan can be raw OCR. Pin the revision id and say what the
  page is. A page that transcludes a scan (`<pages index=…>`) gives a pinned
  edition. The search API throttles bursts; `action=raw` fetches by exact
  title are reliable.
- **Wikimedia Commons.** Per-language song categories: own-work uploads
  under CC BY-SA with VRT permission tickets were the cleanest licensed
  texts found, with the lyric in the file description. Library scans of
  songbooks and collectors' prints: a page image read at full resolution is
  the strongest text pin, and the library's public-domain release covers the
  scan. Per-file copyright tags are a good model for the record's
  `jurisdiction:` line.
- **The Internet Archive.** Page images are reachable as
  `https://archive.org/download/<id>/page/n<leaf>_w1600.jpg`, and the
  `_djvu.xml` file gives the leaf order. Google-digitised items have no
  Arabic OCR: find the leaf through the Latin-script apparatus, then read
  the image. Bibliotheca Alexandrina items (`AAlexandrina-*`) have usable
  Arabic OCR and page images; a modern scholarly edition is a usable pin for
  a public-domain poem when only the poem's text is taken and the edition's
  date is recorded.
- **National-library image servers.** The NDL IIIF API
  (`dl.ndl.go.jp/api/iiif/<pid>/R<page>/full/1600,/0/default.jpg`) for items
  cited by ja.Wikisource; its search API allows about one query per 20
  seconds. Library of Congress notated-music items return JSON with
  `?fo=json`; loc.gov newspaper pages and HathiTrust full text refuse
  scripts, so read them in a browser. IMSLP downloads are gated.
- **Rights holders' own pages,** pinned by an archived capture compared with
  the live page, and **JASRAC's J-WID** as a negative check that no
  collecting society administers a Japanese work (an artist-name search
  made only of punctuation is rejected as empty; search by author name).
- **Genre archives** for dating and credits: todotango.com and
  cancioneros.com for Hispanic song; uta-net and j-lyric for Japanese
  lyricist credits and dates. Cross-check every death year against an
  encyclopaedia or authority record.
- **Author biography pages** (Wikipedia in the song's language, Weblio,
  kotobank, national-library authorities) for the death-date-first method.
- **Library of Congress, Citizen DJ / National Jukebox folk items:**
  identified public domain and explicitly commercial-OK, but US-scoped, so
  verify the source country as well.

## What re-checking the first records taught

- **Japan is life+50 for authors who died before 1968.** The four oldest
  Japanese records had computed Japan's public-domain date with life+70 and
  were twenty years late. Consequence for the URAA: a Japanese lyricist dead
  by 1945 was public domain at home before 1996-01-01 and nothing was
  restored in the US, whatever the publication year; the binding gate is
  then the US date rule, which moves every January.
- **Check the text against a dated print before writing "verbatim".** Six
  of thirteen texts were modern-orthography renderings of the prints their
  records cited, and one had a stanza attested nowhere in its wording, which
  was removed. The records now list every departure.
- **Famous refrains can be authored.** The hook of a "traditional" hit may
  belong to a named lyricist who died recently; look up who wrote the refrain
  before calling the song public domain. song_5 keeps the poem and not the
  refrain.
- **Folk texts need stanza-level provenance.** For a mutable song, say where
  each stanza is attested; an unattested stanza is a text defect even when
  the rights call is unaffected.
- **Write "worldwide" only when it is true,** and make the `jurisdiction:`
  line agree with `residual_exposure:`.
- **Rights in the layers around a text.** A faithful scan of a public-domain
  page creates no new copyright (US: Bridgeman v. Corel; Commons' PD-scan
  policy; UK: Reject Shop v Manners; PRC: no originality). A publisher's
  typographical or layout right (PRC Art. 37, ten years; UK published
  edition, 25 years) expires long before it could matter for an 1890s–1920s
  book and never reaches the words. A faithful transcription has no
  originality, so a Wikisource page's CC BY-SA covers its contributors'
  annotations, not the public-domain text. Library terms of use bind the
  image file, not the words; the corpus holds transcribed text, never
  images. A deterministic character conversion (OpenCC, Apache-2.0 for the
  software) creates no right in its output. A modern edition's added
  vocalization is the one layer that can carry a short related right in some
  EU states (Stage 3, step 5).

## Directions that would broaden the corpus (unverified)

All of these still need the full procedure; none is a finding.

- **English:** a pre-1930 spiritual, gospel or blues standard, a distinct
  register from what is in; traditional ballads.
- **Spanish:** peninsular variety (a traditional Andalusian or Basque song);
  a clean Andean huayno or carnavalito with Quechua words, but it must be
  traditional or pre-1929 to escape the URAA, since named-author
  twentieth-century Andean songs were restored.
- **Japanese:** lyricists who died in or before 1945 with 1929–1930
  publications (Tier 0 under the life+50 rule and the US date rule);
  min'yō from regions other than Hokkaidō; the other songs under the
  song_34–35 grant and the song_32–33 uploader's remaining upload, each on
  the same basis once its lyricist credit is checked. A Japanese text with
  Latin-script English words is still wanted and exists only in Tier L:
  pre-war songs render foreign words in katakana.
- **Mandarin:** early-Republican vernacular poems set to music whose poets
  died before the Tier 0 bound, with scans on zh.Wikisource (check the
  death year against the bound: a 1946 death is Tier 1 until 2027); the
  anonymous popular songs of the 1828 anthology 白雪遺音.
- **Arabic:** the other suites in the 1893 Paris print that song_28 comes
  from, and the other songs in the 1922 collection that song_27's witness
  comes from, are pinned Tier 0 sources; Shawqi's other poems on
  ar.Wikisource (d. 1932).
- **Modern texts for Spanish, Arabic and Mandarin:** systematic searches of
  every open catalogue found no licensed or dedicated text with a clean
  chain (the lyricist as licensor, a published text). The remaining routes
  are a direct CC BY grant requested from a named creator for a named text,
  or public domain by age.
- **New languages:** apply the same gate; the conventions above are per
  script, and a new script needs its layout convention written into this
  file.

## Forks and derived corpora

The developer material (this file, the README, the ledger, the notice, the
records, REUSE.toml, and the selection and arrangement) is CC BY 4.0; the
suggested attribution is in `LICENSE`, Section 2. The texts keep their own
status: the public-domain texts carry no condition, the dedicated and granted
texts none, and song_32 and song_33 are CC BY-SA 4.0, so an adaptation that
includes their text is share-alike and their attribution in `NOTICE.md`
travels with them. When you fork and add songs:

- keep the records, the ledger and the REUSE annotations current for what
  you add, and state your own standard if it differs from the README's;
- do not present your additions as this corpus's determinations, and do not
  attribute your rights calls to its maintainer;
- the tier table's bounds move each January; re-tier before you publish;
- a proposal you make here from a fork still follows Stages 0–6, including
  hard stop 4: the pull request or issue carries the record, the pin and the
  hashes, not the text.
