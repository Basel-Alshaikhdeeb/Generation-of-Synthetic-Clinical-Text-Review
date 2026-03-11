# Generation-of-Synthetic-Clinical-Text-Review
This repository aims at documenting the PRISMA steps of an article titled "Generation of Synthetic Clinical Text: A Systematic Review". This includes the databases used for the search, the search query syntax, retrieved articles, reviewer's judgment and conflict resolution along with risk of bias assessment.

Four main databases have been within the search used including PubMed, ScienceDirect, Scopus, and Web of Science. Two query paradigms have been used for the search; the first query intends to investigate general terms as 

```
synthetic medical text generation
```

whereas the second query was intended to identify derivations within the title as 

```
(generat* OR augment* OR synthetic) AND (medic* OR clinic* OR health*) AND (text* OR record* OR note*)
```

The search has been limited to years 2015 till 2025, in which the search has been conducted on 19th of January 2026. On the other hand, only peer-reviewed articles were targeted. In order to reproduce the results, the following search syntax can be used for each database:

## PubMed
The syntax for general query is:
```
(synthetic medical text generation AND (2015:2025[pdat]) AND (journal article[pt]) NOT (review[pt] OR systematic review[pt] OR meta-analysis[pt] OR books[pt] OR book chapter[pt] OR congresses[pt] OR conference paper[pt] OR editorial[pt] OR letter[pt] OR comment[pt] OR preprint[pt]))
```
which retrieves 121 articles

The syntax for title query is:
```
(("generat*"[Title] OR "augment*"[Title] OR synthetic[Title]) AND ("medic*"[Title] OR "clinic*"[Title] OR "health*"[Title]) AND ("text*"[Title] OR "note*"[Title] OR "record*"[Title]) AND (2015:2025[pdat]) AND (journal article[pt]) NOT (review[pt] OR systematic review[pt] OR meta-analysis[pt] OR books[pt] OR book chapter[pt] OR congresses[pt] OR conference paper[pt] OR editorial[pt] OR letter[pt] OR comment[pt] OR preprint[pt]))
```
which retrieves 261 articles

## ScienceDirect
The syntax for general query is:
```
https://www.sciencedirect.com/search?qs=synthetic+medical+text+generation&tak=%28synthetic+OR+generate+OR+augment%29+AND+%28medical+OR+clinical+OR+health%29+AND+%28text+OR+record+OR+note%29&date=2015-2025&show=100&articleTypes=FLA&lastSelectedFacet=articleTypes
```
which retrieves 155 articles

The syntax for title query is:
```
https://www.sciencedirect.com/search?title=\%28synthetic+OR+generate+OR+augment\%29+AND+\%28medical+OR+clinical+OR+health\%29+AND+\%28text+OR+record+OR+note\%29&date=2015-2025&articleTypes=FLA&lastSelectedFacet=articleTypes
```
which retrieves 41 articles

## Scopus
The syntax for general query is:
```
TITLE-ABS-KEY ( synthetic medical text generation ) AND PUBYEAR > 2014 AND PUBYEAR < 2026 AND ( LIMIT-TO ( DOCTYPE , "ar" ) )
```
which retrieves 51 articles

The syntax for title query is:
```
TITLE ( "generat*" OR "augment*" OR synthetic ) AND TITLE ( "medic*" OR "clinic*" OR "health*" ) AND TITLE ( "text*" OR "note*" OR "record*" ) AND PUBYEAR > 2015 AND PUBYEAR < 2025 AND ( LIMIT-TO ( DOCTYPE , "ar" ) )
```
which retrieves 198 articles

## Web of Science
The syntax for general query is:
```
https://www.webofscience.com/wos/woscc/summary/cf75691a-b26f-4a1c-bc0f-4be7c8c7dd7e-0199bc69c1/relevance/1
```
which retrieves 87 articles

The syntax for title query is:
```
https://www.webofscience.com/wos/woscc/summary/3398c601-2f0f-4621-88f4-bb623a39475e-0199bc4318/relevance/1
```
which retrieves 234 articles
