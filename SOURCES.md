# Toda Language Dataset — Sources & Notes

Toda (ISO 639-3: `tcx`, Glottolog: `toda1252`) is a Dravidian language spoken by
roughly 1,000–1,600 people in the Nilgiri Hills of Tamil Nadu, India. It is
severely under-documented: there is no large digitized corpus, no standard
orthography, and no mainstream bilingual dictionary in print or online. Almost
everything known about it academically traces back to a handful of works.

## Primary academic sources (not directly machine-readable, but the ultimate
authority behind everything in this dataset)

- **Emeneau, Murray B. 1984. *Toda Grammar and Texts*.** Philadelphia:
  American Philosophical Society, Memoirs Series 155. xiii+426pp. — The
  foundational grammar, built from fieldwork in 1935–1938; includes ~260
  transcribed ritual songs/texts. This is the single most authoritative source
  on Toda morphology and syntax.
- **Sakthivel, S. 1976. *Phonology of Toda with Vocabulary*.** Annamalainagar:
  Annamalai University. 382pp.
- **Nara, Tsuyoshi & Peri Bhaskararao. 2001. *Toda Vocabulary: A Preliminary
  List*.** Endangered Languages of the Pacific Rim, A3-002. Osaka: ELPR.
- **Burrow, T. & M.B. Emeneau. 1984. *A Dravidian Etymological Dictionary*,
  2nd ed.** Oxford University Press. (Comparative Dravidian cognates.)

These are the sources every other resource on Toda ultimately cites. They are
copyrighted, out-of-print or hard-to-access academic monographs, so I did not
reproduce large passages from them directly.

## What's actually in this dataset

The vocabulary, grammar rules, and parallel sentences in `toda_vocabulary.csv`,
`toda_grammar_rules.csv`, and `toda_parallel_sentences.csv` were extracted from
**a secondary academic-style summary site**:

> *Toda Language* (blog), https://todalang.wordpress.com — a linguistics
> project site with dedicated Vocabulary, Morphology, and Syntax pages, each
> transcribing real word lists, case paradigms, verb paradigms, and example
> sentences directly from Emeneau (1984), Sakthivel (1976), and Nara &
> Bhaskararao (2001), with page-level citations throughout.

Every row includes a `Source` column pointing back to this chain of
attribution so you can trace any entry to the original grammar/vocabulary if
needed. Toda forms use Emeneau-style IPA-based transcription (e.g. `ɫ`, `θ`,
`s̠`, dot-under for retroflexes) rather than a standardized orthography,
because none is standardized — a proposal for a >50-character script exists
but is not widely adopted.

## Other resources worth pursuing if you need more data

- **The Endangered Languages Project / UCLA Phonetic Laboratory** —
  http://www.endangeredlanguages.com/lang/5103/guide — audio recordings of
  Toda vocabulary and phonetics.
- **Central Institute of Indian Languages (CIIL), Scheme for Protection and
  Preservation of Endangered Languages (SPPEL)** — has done digital
  archiving of Toda grammar/core vocabulary; check ciil.org for access.
- **Spajić, Ladefoged & Bhaskararao (1994, 1996)** — phonetic studies
  specifically on Toda's rhotics/trills, useful if you need phonology data.
- Emeneau's book itself (scanned/preview on Google Books) if you need to
  go past what's summarized here — but note it's a purchasable academic
  monograph, not freely reproducible in bulk.

## Honest limitations

- This is a **small, hand-curated sample** (roughly 85 vocabulary items, 16
  grammar rules, 12 parallel sentences) — not a corpus. Toda is genuinely
  this scarce online; there is no equivalent of a "Toda Wiktionary" or open
  parallel corpus at scale.
- A few glosses in the parallel-sentence set look internally inconsistent
  (e.g. a literal-sounding fragment vs. a free translation) because they're
  transcribed as-is from field-linguistics texts, which often mix literal
  and free translation conventions. I kept them faithful to the source
  rather than "cleaning" them into something that looks more polished but
  isn't accurate.
- POS tags for the vocabulary list are my own light annotation layer on top
  of the source glosses (the sources don't tag POS explicitly for every
  word), so treat that column as a helpful approximation, not a citation.
- If your notebook needs hundreds/thousands of parallel sentences, that
  volume doesn't currently exist in the public domain for Toda — you'd need
  direct access to Emeneau's 260 transcribed texts or a partnership with
  CIIL/field linguists working with the Toda community today.
