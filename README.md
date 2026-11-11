# CBAM planning aid — static pages

What the EU's Carbon Border Adjustment Mechanism asks of an importer, the Commission's defaults and 2026
certificate prices, a worked example, and a **fictional** importer's ledger of tube and pipe fittings (CN 7307)
worked through. Published by ordo-markets. Plain static files for GitHub Pages: no server, no tracking, no data
leaves the reader's browser.

**Disclaimer v1.3 (2026-11-09).** This page is a free planning and verification aid, provided as is and used at your own risk. It is not a source for a CBAM declaration: the values filed are the European Commission's published defaults as presented in the CBAM Registry, which govern where anything here differs. Nothing on this page is legal, tax or customs advice, and, to the extent permitted by law, no warranty is given for accuracy, completeness or fitness for any purpose. Every regulatory statement shown cites the official text it rests on, quoted verbatim where in quotation marks, with its retrieval date; check the source before relying on it. Use of this page creates no obligation on either side.

## What is on the pages, and where it comes from

| page | content | basis |
|---|---|---|
| What CBAM asks | the explainer C1–C5 | 37 quotes from the official texts, retrieved 2026-11-02 |
| Worked example | one pilot line, step by step | Commission defaults, the Commission's Q1 2026 price, arithmetic |
| CN 7307 pilot (fictional) | 10 invented lines, 4 invented importers | the same; the calculation reproduces the Commission's Guidance No. 4 and No. 5f examples |
| Your ledger | your own CSV ledger, computed in your browser and sent nowhere: per line, the 50-tonne threshold per importer, totals, 2026–2034, suppliers, a results CSV | the same tables, bundled; the calculation is a port of the Python calculator, tested field by field against it (P9) |
| 2026 to 2034 | the fictional pilot re-dated year by year: cost per tonne, the two rules that drive it, why 2031–2033 are open | the same |
| Sources and corrections | every quote with its official URL, retrieval date and document sha256; the correction log | `cbam_ground_truth_2026-11-02.json` |

Certificate prices: Q1 2026 €75.36, Q2 €75.28, Q3 €82.32; Q4 is
published by the Commission on 2027-01-04 (https://taxation-customs.ec.europa.eu/carbon-border-adjustment-mechanism/price-cbam-certificates_en, retrieved
2026-11-06).

Pages: https://ordo-markets.github.io/cbam-planning-aid/ ·
Impressum, the full disclaimer (liability for content and links, copyright and licences) and the privacy notice:
on the pages (`#/impressum`, `#/privacy`), linked from every page's footer. The pages set no cookie, store nothing in
the browser and load nothing from another provider.

**Not on the pages:** no electricity default from Annex III to Implementing Regulation (EU) 2025/2621 (IEA data,
licensed for non-commercial use only), no model output of any kind, no real company.

## Related

- Essay: [How to count a German power plant twice](https://ordomarkets.substack.com/p/how-to-count-a-german-power-plant)
- Data and reproduction kit: [German-Fleet-Essay (data and reproduction kit)](https://github.com/ordo-markets/German-Fleet-Essay)

## Licences

- The site's own code (the JavaScript in `assets/` that is not a third-party library): MIT, `LICENSE`.
- Our text and the fictional pilot: CC BY 4.0, `LICENSE-CONTENT`.
- Quoted official texts remain under their publishers' terms; each quote names its source.
- Third-party libraries in the bundle keep their own licences: `THIRD-PARTY.md` (26 packages).

## Corrections

2026-11-09: Before publication of the ledger calculator: a line whose free allocation adjustment exceeds its embedded emissions showed a negative certificate figure. It now shows 0, as Implementing Regulation (EU) 2025/2620, recital 16, reads that case ("no CBAM certificates would be due"); the excess is shown beside the line and is not set against another good, which no quoted text establishes. Seven quotes were added to the Sources page, each dated 2026-11-09. No published figure changes: the pilot has no such line. Report an error by opening an issue; it is
checked against the cited official text, and if the text wins the item is corrected and logged on the Sources page.

Built from the private repository's commit `b11a6c4`; this repository carries no history from it.
