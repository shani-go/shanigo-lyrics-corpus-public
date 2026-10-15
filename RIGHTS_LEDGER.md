# Song lyrics corpus — rights ledger (public release)

One row per released song: its rights basis, tier and release status, with a
link to its rights record. The record (`songs/<slug>.rights.md`) is
authoritative, with the evidence, the jurisdiction checked and the caveats.
This ledger is the index. The standard the rows apply, the admission gate and
the jurisdiction tiers, is in [`README.md`](README.md).

Verification is **human-led**: `verified_by = developer` means the developer
confirmed the public-domain or licence status. Automated research assisted
(each record says where Claude Code drafted), but it was not the authority
for any rights call.

## Standard

- **Admission gate:** lyrics public domain in the **United States AND the
  country of origin**, or licensed for commercial and educational use and
  redistribution.
- **Jurisdiction tier per song** (`README.md`, "Jurisdiction tiers"): **Tier 0
  — universal** (anonymous or traditional, or the lyricist died before the
  year's Tier 0 bound: 1946 in 2026); **Tier 1 — life+70 has run**; **Tier 2
  — US and origin only**; **Tier L — licensed or dedicated**. Tiers were
  computed on **2026-09-29** and re-checked for this release on
  **2026-10-14**. A song can only rise.
- **What a tier allows:** Tier 0 and Tier L allow any use, including public
  release. Tier 1 and Tier 2 songs are excluded from public release.
- **This release** holds the 27 Tier 0 songs and the 7 Tier L songs.
- Tier assignments were drafted by Claude Code and **confirmed by the
  developer on 2026-09-29**. song_29–song_35 are Tier L: song_29–31 by the
  author's public-domain dedication, song_32–33 under CC BY-SA 4.0, and
  song_34–35 by a rights holder's public-domain grant. All other rows are
  Tier 0.

## Ledger

All rows: allowed uses = commercial, educational, redistribution (required for
admission). "Residual exposure" lists the countries where the lyrics are still
protected under the strict no-comparison reading, and until when. The
"verified" column shows the original rights call and its 2026-09-29 upgrade;
every row was re-verified on 2026-10-14 for this release, as each record's
`verified_on` states, together with any check that rests on the earlier
verification (song_1, song_17, song_26 and song_27).

| slug | title | lang | genre | rights_basis | jurisdiction checked | tier (2026) | residual exposure → tier changes | release | verified | record |
|---|---|---|---|---|---|---|---|---|---|---|
| song_0 | Early One Morning | en | traditional English folk | public-domain (anonymous, pre-1929; lyrics in print from 1787) | UK source + US | **0 universal** (anonymous) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_0.rights.md](songs/song_0.rights.md) |
| song_1 | The John Brown Song (John Brown's Body / "Glory, Hallelujah") | en | US Civil War marching song | public-domain (the six verses are William Weston Patton's, d. 1889 — Chicago Tribune 1861-12-16 / Root & Cady, Chicago; the chorus is the anonymous 1861 soldiers' song; pre-1929) | US source + generally | **0 universal** (d. 1889; chorus anonymous) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_1.rights.md](songs/song_1.rights.md) |
| song_3 | El cant dels ocells | ca (Catalan) | traditional Catalan Christmas carol | public-domain (anonymous/traditional; centuries old) | Catalonia/Spain + US | **0 universal** (anonymous) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_3.rights.md](songs/song_3.rights.md) |
| song_4 | La Cucaracha | es (Mexican) | traditional folk / Revolution-era song — 3 stanzas (the unattested fourth dropped 2026-09-29) | public-domain (anonymous/traditional) | Mexico + US | **0 universal** (anonymous) | none under copyright; Mexico folklore-regime note (LFDA Arts. 157–160, 2020 reform — commercial use in Mexico; added 2026-10-14, see record) | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_4.rights.md](songs/song_4.rights.md) |
| song_5 | Versos sencillos — three quatrains (the verses sung as "Guantanamera") | es (Cuban) | 19th-c Cuban poetry (Martí's octosyllabic quatrains) — the song's refrain lines, Joseíto Fernández's (d. 1979), were removed 2026-09-29 | public-domain (José Martí d. 1895; Versos sencillos, New York 1891, checked against the first edition 2026-09-29) | Cuba + US | **0 universal** (d. 1895) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_5.rights.md](songs/song_5.rights.md) |
| song_6 | Donguri Korokoro (どんぐりころころ) | ja | Taishō-era children's song (dōyō/shōka) | public-domain (Aoki Nagayoshi d. 1935 → JP life+50 PD since 1986 — corrected 2026-09-29 from a life+70 miscalculation; published 1921/22 → US pre-1929) | Japan + US | **0 universal** (d. 1935 < 1946) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_6.rights.md](songs/song_6.rights.md) |
| song_8 | ソーラン節 (Sōran Bushi) | ja | traditional min'yō (Hokkaidō herring-fishery work song) | public-domain (anonymous/communal 北海道民謡) | Japan + US | **0 universal** (anonymous) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_8.rights.md](songs/song_8.rights.md) |
| song_9 | 波浮の港 (Habu no Minato) | ja | Taishō/early-Shōwa ryūkōka (民謡調 modern port ballad) | public-domain (Noguchi Ujō d. 1945 → JP life+50 PD since 1996 — corrected 2026-09-29 from a life+70 miscalculation; published 1923/1924 (two verses; the 1928 records carry all five) → US pre-1929) | Japan + US | **0 universal** (d. 1945 < 1946; Colombia's life+80 ran out 2025-12-31) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_9.rights.md](songs/song_9.rights.md) |
| song_10 | Amazing Grace ("Faith's Review and Expectation") | en | Christian hymn / spiritual | public-domain (John Newton d. 1807; published 1779; the file's spelling is the 1840 Glasgow edition's — see record) | UK source + US | **0 universal** (d. 1807) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_10.rights.md](songs/song_10.rights.md) |
| song_11 | ラッパ節 (Rappa-bushi) | ja | Meiji/Taishō enka (street-singer social satire) | public-domain (Soeda Azenbō d. 1944 → JP life+50 PD since 1995 — corrected 2026-09-29 from a life+70 miscalculation; created 1904–05 → US pre-1929) | Japan + US | **0 universal** (d. 1944 < 1946) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_11.rights.md](songs/song_11.rights.md) |
| song_12 | Mi noche triste ("Percanta que me amuraste") | es (Argentine / lunfardo) | Argentine tango — first tango canción (1917) | public-domain (Pascual Contursi d. 1932 → life+70 PD since 2003; published 1917 → US pre-1929) | Argentina + US | **0 universal** (d. 1932 < 1946) | none | public release eligible | developer, 2026-09-21 (record upgrade 2026-09-29 confirmed) | [song_12.rights.md](songs/song_12.rights.md) |
| song_13 | 教我如何不想她 (Jiao Wo Ru He Bu Xiang Ta) | zh | early vernacular (白話) art song — 1920 poem, set to music 1926 | public-domain (Liu Bannong d. 1934 → China life+50 PD since 1985, before the URAA date; published 揚鞭集 1926 → US pre-1929) | China (source) + US | **0 universal** (d. 1934 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_13.rights.md](songs/song_13.rights.md) |
| song_14 | 送別 (Song Bie) — stanza 1 only | zh | 學堂樂歌 school song / farewell (c. 1915; published 1927) | public-domain (Li Shutong d. 1942 → China life+50 PD since 1993; published 中文名歌五十曲 1927 → US pre-1929) | China (source) + US | **0 universal** (d. 1942 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_14.rights.md](songs/song_14.rights.md) |
| song_15 | 海韻 (Hai Yun) | zh | narrative / dialogue art song text (1925; choral setting 1927) | public-domain (Xu Zhimo d. 1931 → China life+50 PD since 1982; published 1925 → US pre-1929) | China (source) + US | **0 universal** (d. 1931 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_15.rights.md](songs/song_15.rights.md) |
| song_16 | 勉女權歌 (Mian Nü Quan Ge) | zh | late-Qing women's-rights reform song (1907) | public-domain (Qiu Jin d. 1907; published 中國女報 1907) | China (source) + US | **0 universal** (d. 1907) | none | public release eligible | developer, 2026-09-29 | [song_16.rights.md](songs/song_16.rights.md) |
| song_17 | 小白菜兒 (Xiao Bai Cai'r) | zh (Beijing dialect, 兒化) | traditional children's folk lament (1896 print) | public-domain (anonymous/traditional; Vitale, *Pekinese Rhymes*, Peking 1896) | China (source) + US | **0 universal** (anonymous) | none | public release eligible | developer, 2026-09-29 | [song_17.rights.md](songs/song_17.rights.md) |
| song_18 | 水牛兒 (Shui Niu'r) | zh (Beijing dialect, 兒化) | traditional nursery song (1896 print; also Headland 1900) | public-domain (anonymous/traditional; Vitale, *Pekinese Rhymes*, Peking 1896) | China (source) + US | **0 universal** (anonymous) | none | public release eligible | developer, 2026-09-29 | [song_18.rights.md](songs/song_18.rights.md) |
| song_19 | يا جارة الوادي (Ya Jarat al-Wadi) — verses 10–22 of زحلة | ar (Modern Standard Arabic) | neo-classical love poem sung as a 1928 art song (Abdel Wahab; later Fairuz) | public-domain (Ahmad Shawqi d. 1932 → Egypt life+50 PD since 1983, before the URAA date; song recorded 1928) | Egypt (source) + US | **0 universal** (d. 1932 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_19.rights.md](songs/song_19.rights.md) |
| song_20 | إرادة الحياة (Iradat al-Hayah) | ar (MSA, mostly vocalized) | Romantic MSA poem, sung and recited; two verses in Tunisia's anthem; verse 9 confirmed against the 1955 diwan page (2026-09-29) | public-domain (Abu al-Qasim al-Shabbi d. 1934 → Tunisia/Egypt life+50 PD since 1985, before the URAA date; published Apollo, Cairo 1933) | Tunisia + Egypt + US | **0 universal** (d. 1934 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_20.rights.md](songs/song_20.rights.md) |
| song_21 | أراك عصي الدمع شيمتك الصبر (Araka Asiyya al-Dam') | ar (Classical Arabic) | 10th-c. qasida sung by Umm Kulthum (1926, 1944, 1965) — the archaic-register fixture; Wikisource text with one correction (line 54 النصر) after a three-witness check, 2026-09-29 | public-domain (Abu Firas al-Hamdani d. 968) | everywhere by age | **0 universal** (pre-modern) | none | public release eligible | developer, 2026-09-29 | [song_21.rights.md](songs/song_21.rights.md) |
| song_22 | أعطني الناي (Give Me the Flute) — 8 couplets of المواكب | ar (MSA) | philosophical poem (New York 1919) → Fairuz art song | public-domain (Kahlil Gibran d. 1931 → Lebanon life+50 PD 1982; first published in the US 1919 → US PD by date) | US (country of origin) + Lebanon | **0 universal** (d. 1931 < 1946) | none | public release eligible | developer, 2026-09-29 | [song_22.rights.md](songs/song_22.rights.md) |
| song_23 | النيل نجاشي (al-Nil Nagashi) | ar (Egyptian Arabic, Cairene colloquial) | 1933 film song (Abdel Wahab) — the MASRI dialect fixture | public-domain (Ahmad Shawqi d. 1932 → Egypt life+50 PD since 1983, before the URAA date; first performed 1933, never US-protected) | Egypt (source) + US | **0 universal** (d. 1932 < 1946) | none | public release eligible (text pin is website witnesses only — see record) | developer, 2026-09-29 | [song_23.rights.md](songs/song_23.rights.md) |
| song_24 | قال المزيان تصف لي زيني (malhun qasida) | ar (Moroccan Darija, malhun) | Moroccan malhun ghazal with refrain (printed Paris 1902) — the DARIJA fixture | public-domain (Qaddur al-Alami of Meknes d. c. 1850; Sonneck, Chants arabes du Maghreb I, 1902) | Morocco + US | **0 universal** (19th-c. author) | none | public release eligible | developer, 2026-09-29 | [song_24.rights.md](songs/song_24.rights.md) |
| song_25 | تريد الهوى لك على ما تريد (a Kuwaiti sawt) | ar (Gulf / Kuwaiti Arabic, Nabati) | Kuwaiti sawt khayali in the poet's own melody — the KHALEEJI fixture | public-domain (Abdullah al-Faraj d. 1901; diwan printed Bombay 1919) | Kuwait + US | **0 universal** (d. 1901) | none for the poem; doubtful EU edition-right note on the kept vocalization if it is the 2001 edition's (Germany to 2026-12-31, EU maximum 2031-12-31) — developer decision 2026-10-14: ship as is (see record) | public release eligible | developer, 2026-09-29 | [song_25.rights.md](songs/song_25.rights.md) |
| song_26 | يا حمامة الوادي (Jerusalem lullaby) | ar (Palestinian Arabic, Jerusalem) | traditional lullaby — the SHAAMI dialect fixture; Arabic file is a project RENDERING of the 1901 transliteration (kept verbatim as song_26.translit.txt) | public-domain (anonymous/traditional; Dalman, Palästinischer Diwan, Leipzig 1901, pp. 165–166; collector d. 1941) | everywhere by anonymity and age (folklore regimes noted in the record) | **0 universal** (anonymous) | none under copyright; folklore-regime note | public release eligible | developer, 2026-09-29 | [song_26.rights.md](songs/song_26.rights.md) |
| song_27 | عدّيك المياس / دق الباب فتحتله (Jerusalem love song) | ar (Palestinian Arabic, Jerusalem) | traditional love song — second SHAAMI fixture; Arabic file is a project RENDERING of the 1922 transliteration (kept verbatim as song_27.translit.txt) | public-domain (anonymous/traditional; Stephan, JPOS 2 (1922) p. 229; collector d. 1949) | the words: everywhere by anonymity and age; the 1922 witness (Stephan d. 1949) adds no authored layer to the committed files, so his Colombia & Equatorial Guinea term (to 2029-12-31) is not engaged (witness note raised and closed 2026-10-14; folklore regimes noted in the record) | **0 universal** (anonymous) | none under copyright; folklore-regime note | public release eligible | developer, 2026-09-29 | [song_27.rights.md](songs/song_27.rights.md) |
| song_28 | حمل زجل عشق (Bouriant no. 15, a Cairene street-singer zajal) | ar (Egyptian Arabic, Cairene zajal register) | 19th-century Cairo zajal in six sections, five of them labelled (the opening مطلع unlabelled; three أدوار, دور المديح, دور الاستشهاد) — second MASRI fixture, with a pinned 1893 print; section labels kept as lines, print spacing kept | public-domain (poet عبد الوهاب ابن يوسف, known only from his signature stanza — unidentified-author term from 1893 publication expired everywhere by 1993; on a life basis d. before 1946 is the only realistic case; Bouriant, Chansons populaires arabes en dialecte du Caire, Paris 1893, pp. 71–72) | Egypt (source) + US, and everywhere by age | **0 universal** (unidentified author, 1893 print) | none | public release eligible | developer, 2026-09-29 | [song_28.rights.md](songs/song_28.rights.md) |
| song_29 | Pollution | en | 1960s satirical cabaret / topical song (1965) | public-domain — AUTHOR DEDICATION (Tom Lehrer, 1928–2025; all rights relinquished 2020-10, formal disclaimer 2022-11-26) | US source; dedication worldwide | **L licensed/dedicated** | none by dedication (express permission grant where abandonment is not recognised) → no change | public release eligible | developer, 2026-09-29 | [song_29.rights.md](songs/song_29.rights.md) |
| song_30 | The Elements (+ 2020 addendum "Elements 103 to 118") | en | comic patter / list song (1959; four lines added 2020) | public-domain — AUTHOR DEDICATION (Tom Lehrer; as song_29; addendum separately tagged PD on Commons); tune Sullivan 1879, PD by age, not committed | US source; dedication worldwide | **L licensed/dedicated** | none by dedication → no change | public release eligible | developer, 2026-09-29 | [song_30.rights.md](songs/song_30.rights.md) |
| song_31 | Te Amo | en+es (bilingual duet: HE part Spanish, SHE part English) | comic serenade / duet with role labels (1950s, date unconfirmed) | public-domain — AUTHOR DEDICATION (Tom Lehrer; as song_29; sheet credits "words and music by Tom Lehrer (with thanks to Munro Edmonson)" — acknowledgement, not co-authorship, accepted by the developer) | US source; dedication worldwide | **L licensed/dedicated** | none by dedication → no change | public release eligible | developer, 2026-09-29 | [song_31.rights.md](songs/song_31.rights.md) |
| song_32 | テント村宣言 (Tent Village Declaration) | ja | 1991 grassroots anti-nuclear prayer / protest song (関西電力前脱原発テント村) | CC BY-SA 4.0 (lyricist 奥村悦夫; music by the Commons user Toach japan; Commons {{self\|cc-by-sa-4.0}} backed by VRT permission tickets 2020122610000481 and 2020122610000721, the second sent by the lyricist himself) | Japan (source); licence worldwide | **L licensed/dedicated** | none while the licence stands; share-alike rides on adapted artefacts → no change | public release eligible with attribution and licence notice | developer, 2026-09-29 | [song_32.rights.md](songs/song_32.rights.md) |
| song_33 | 南島大橋いかだレース テーマソング (Nantō Bridge Raft Race theme song) | ja | 1992 community festival anthem (南島町, Mie) | CC BY-SA 4.0 (words and music by the Commons user Toach japan; VRT permission ticket 2020061710005558) | Japan (source); licence worldwide | **L licensed/dedicated** | none while the licence stands; share-alike rides on adapted artefacts → no change | public release eligible with attribution and licence notice | developer, 2026-09-29 | [song_33.rights.md](songs/song_33.rights.md) |
| song_34 | 1998- | ja | 2010s idol pop / shoegaze-pop (・・・・・・・・・; first performed 2017; album『 』2018) | public-domain — RIGHTS-HOLDER GRANT (dots.tokyo/PD/, announced 2019-04-12: no permission, reporting, payment or attribution; modification and commercial use allowed — CC0-equivalent; the lyricist みきれちゃん is a member of the issuing management; JASRAC administers none of the titles) | Japan (source); grant worldwide, operating as a licence where abandonment is not recognised | **L licensed/dedicated** | none by grant → no change | public release eligible | developer, 2026-09-29 | [song_34.rights.md](songs/song_34.rights.md) |
| song_35 | トリニティダイブ (Trinity Dive) | ja | 2010s idol pop (・・・・・・・・・; first performed 2017; album『 』2018, track 3) | public-domain — RIGHTS-HOLDER GRANT (as song_34; lyricist みきれちゃん) | Japan (source); grant worldwide | **L licensed/dedicated** | none by grant → no change | public release eligible | developer, 2026-09-29 | [song_35.rights.md](songs/song_35.rights.md) |

**Accepted 2026-09-29:** song_13–song_18 (Mandarin Chinese), song_19–song_25
(Arabic) and song_26–song_27 (the two Shaami fixtures, Arabic renderings of
pre-1929 transliterated witnesses), all Tier 0. The developer confirmed the
values screen, the rights analysis and the cross-check results. In song_26 and
song_27 the Arabic text is a project rendering, and the verbatim
transliteration witness sits beside each.

**Accepted 2026-09-29 (second batch):** song_29–song_31 (Tom Lehrer:
Pollution, The Elements with its 2020 addendum, and the bilingual en/es Te
Amo), all **Tier L** under the author's public-domain dedication of 2020-10 /
2022-11-26. The developer confirmed the values screen and the rights analysis.
The texts were checked against the page images of the author's own lyric
sheets.

**Accepted 2026-09-29 (third batch):** song_32–song_35 (Japanese, all **Tier
L**). song_32 テント村宣言 (1991) and song_33, the 南島大橋いかだレース theme
song (1992), are CC BY-SA 4.0 from Wikimedia Commons, with VRT permission
tickets. They are the corpus's first share-alike rows, so any adapted artefact
that includes their text must carry a compatible licence. song_34 1998- and
song_35 トリニティダイブ (2017) rest on the idol group ・・・・・・・・・'s
rights-holder public-domain grant (dots.tokyo/PD/, 2019-04-12;
CC0-equivalent; the songs are outside JASRAC administration). The developer
confirmed the values screen and the rights analysis. They judged the
management's grant sufficient for its own in-house lyricist, and Commons'
VRT process sufficient corroboration.

**Accepted 2026-09-29 (fourth batch):** song_28 (Arabic, **Tier 0**), a
two-page love zajal from Urbain Bouriant's 1893 Paris print of a Cairo street
singer's manuscript, transcribed from the scan images and pinned to
pp. 71–72. The poet is known only from the signature stanza, so the term is
publication-based and long expired. The developer agreed the Tier 0 call on
both routes, kept the print's word spacing and the five section labels, and
accepted it as the corpus's second Masri fixture beside song_23.

**Renumbered 2026-09-29:** the seven Tier L songs were accepted as
song_40–46 and became song_29–35, so that the slugs follow song_28 without a
gap. Each record's `notes` names its original slug.

**Record upgrade 2026-09-29 (confirmed by the developer the same day):** the
records first verified on 2026-09-21 (song_0–song_12) were reviewed against
the standard of the later records. Claude Code redrafted them with an
`edition:` pin (source revision or scan, line and stanza counts, every
normalisation), a `composer:` line, full birth and death dates, a values
screen where one was missing, and the dated witnesses found: Chappell 1859 for
song_0, the Chicago Tribune of 1861-12-16 for song_1, Pelay Briz 1874 for
song_3, the 1891 first edition for song_5, the 1921/22 first print and the
1949 textbook for song_6, the 1924 雨情民謡百篇 for song_9, and the 1779 and
1840 Olney Hymns for song_10. Each record keeps the developer's 2026-09-21
verification and the developer's confirmation of the additions. The review
corrected four facts, all reflected in the rows above:

1. The Japanese records (song_6, 9 and 11) had
   computed Japan's public-domain date with life+70. The term that governed
   authors who died before 1968 was life+50, because the 2018 extension did
   not revive expired works. The dates are 1986, 1996 and 1995, twenty years
   earlier than stated. No tier changed.
2. song_1's six verses are William Weston Patton's (d. 1889), not anonymous.
   Tier 0 holds.
3. song_5's refrain lines are Joseíto Fernández's (d. 1979), not traditional.
   The developer had them removed, so song_5 holds Martí's text only (14
   lines) and was retitled.
4. song_10's text is the 1840 edition's state, not the 1779 print's.

Five texts (song_3, 5, 6, 9 and 10) are modern-orthography
renderings of dated prints rather than verbatim copies. The developer kept
them as they are: orthographic normalisation of a public-domain text is not
original authorship, and a Wikisource page's CC BY-SA banner does not attach
to a transcription of a public-domain text. song_4's fourth stanza was
attested nowhere in its wording and was dropped, so song_4 has 3 stanzas and
14 lines. Five pins need a source in hand and stay open: song_1's Tribune
page, song_4's stanza 3, song_8's and song_11's dated prints, and song_12's
score. None affects a rights call.

**Release review 2026-10-14:** before this release was prepared, the records of
song_4 (the Mexican folklore-regime note), song_25 (the vocalization layer;
the developer decided to ship it as is), song_27 (the 1922 witness note,
raised and closed) and song_31 (the authorship basis) were corrected or
extended. Each record's notes give the detail under that date.

## Open items

None that affects a rights call. The five source pins listed under "Record
upgrade 2026-09-29" above (song_1, 4, 8, 11 and 12) and song_9's first-print
pin stay open as provenance items.

## Releases

Each release adds a row: the date, the platform, the set by slug and tier,
and who approved it.

| date | platform | set (slug: tier) | approved by |
|---|---|---|---|
| 2026-10-14 | GitHub (https://github.com/shani-go/shanigo-lyrics-corpus-public), tag `v2026-10-14` | 34 songs, tier snapshot of 2026-10-14 — Tier 0 (27): song_0, 1, 3, 4, 5, 6, 8, 9, 10, 11, 12, 13–28; Tier L (7): song_29–31 (author's dedication), song_32–33 (CC BY-SA 4.0), song_34–35 (rights holder's grant) | shani (developer) |

## Notes that apply across rows

- **Only lyrics are included.** Sound recordings and music (including song_6's
  separately copyrighted music, composer d. 1959) are not part of this release
  and do not affect these records.
- **Text version matters.** Each record covers the specific public-domain or
  licensed text version taken from its cited source; traditional songs have
  many variants. A source site's page furniture and annotations are not part
  of the lyric text.
- **Composition: 34 songs.** English 5 (song_0, 1, 10, 29, 30); Spanish 3
  (song_4, 5, 12) and Catalan 1 (song_3, `language:` `ca`); Japanese 8
  (song_6, 8, 9, 11, 32–35); Mandarin Chinese 6 (song_13–18); Arabic 10
  (song_19–28); bilingual English/Spanish 1 (song_31, `language:` `en+es`).
  Slugs are 0-indexed, not contiguous and not grouped by language. Use each
  record and this ledger, never the number, to tell what a slug is.
- **Chinese songs** have two files: `song_<n>.txt`, the simplified edition
  (an OpenCC conversion recorded in the record's `edition:` field), and
  `song_<n>.zh-hant.txt`, the traditional source edition, verbatim.
- **Arabic files** hold one hemistich per line, with vocalization exactly as
  in the source; song_26 and song_27, which are project renderings, follow
  their records' `edition:` fields instead. song_24 writes the print's Maghrebi qāf and fāʾ as standard
  ق and ف, as its record says. song_26 and song_27 carry
  `song_<n>.translit.txt`, the verbatim 1901 and 1922 transliteration that
  their Arabic file renders.
- **Tier L rows:** song_29–31 and song_34–35 are public domain by a dedication
  or grant, not by age, so their records cite the grant instead of a death
  year. song_32–33 are CC BY-SA 4.0, and the share-alike condition rides on
  any adapted artefact that includes their text.
