# Wind-Resilient Truck–UAV Delivery — OMEGA Lab project page

Project page for **Energy-Aware Wind-Resilient Routing for Truck-Assisted Multi-UAV Delivery under
Wind Uncertainty** (EWR), in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2608.11641>
- Code: <https://github.com/LITIANSHUN/The-EWR-UAV-Routing>
- Page: <https://omega-hkustgz.github.io/projects/wind-resilient-uav-delivery/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/`; there is no build step. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs
node tools/serve.mjs     # look at it locally
```

Every pull request gets a preview link, posted on the pull request. A push to `main` asks the
lab site to republish.

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2608.11641v1 (12 Aug 2026). The text paraphrases the abstract and Sections I, III, IV, V and VI; it adds no claims. The arXiv record states no venue, so the citation is `@misc`. |
| `routing.webp`, `framework.webp`, `success-sensitivity.webp`, `return-safety.webp` | Figs. 2, 1, 3 and 4 of the paper, rendered from the arXiv source PDFs at 2400 px wide (`pdftoppm -cropbox`, then `cwebp -q 90`). A stray export mark in the bottom-left corner of the Fig. 2 file, outside the plots, is painted white in `routing.webp`. `social.jpg` is Fig. 2 on a 1200 × 630 canvas for link previews. |
| Wind-log replay and scalability tables, headline numbers | Tables III and II of the paper, copied from the LaTeX source. "Approximately 92%" and "above 75%" are the paper's own reading of Fig. 3(a) in Section V-C. UAV parameters are from Table I. |
| Evidence labels | Fig. 2 is a routing visualization from the simulation (Simulation). Every experiment in the paper is a log-replay simulation; the "real-world" wind log of Table III is recorded ASOS weather-station wind replayed in simulation. |
| Code button | The authors' public repository: a Python reference implementation with a synthetic demo. Its README marks ATS and ASOS preprocessing, the paper's experiment split files and reproduction seeds as "Coming soon". |
| Earlier preprint (one sentence in Scope) | arXiv 2604.13441 by the same authors, linked without claiming a version relationship; neither paper states one. |

Not on the page because no public material exists: a demo video, flight-test footage (the paper
reports simulation only), the experiment data and seeds behind the tables, and a published-venue
record or DOI on arXiv.
