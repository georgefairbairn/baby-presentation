# Let's Make a Baby!

A reveal.js presentation covering everything you need to know about starting a family - pregnancy, birth, the first year, and finances.

**Live site:** https://georgefairbairn.github.io/baby-presentation/

37 slides, roughly 40 minutes, about 160 key presses end to end.

## Running locally

```bash
npm install
open index.html
```

## Speaker notes

See [TALK-TRACK.md](TALK-TRACK.md) for talking points for each slide. Slide
numbers in the talk track match the deck exactly. The slides carry the facts,
the talk track carries what you say.

## Structure

`css/custom.css` holds a small set of components that every slide is built from.
There are no inline styles in the deck, so changing a component changes it
everywhere.

| Component | What it's for |
| --- | --- |
| `.cols` + `.panel` | Titled columns of items, the workhorse layout |
| `.tiles` | A grid of small cards |
| `.stats` | Big-number comparison cards |
| `.triage` | Red / amber / green urgency columns |
| `.track` | A horizontal timeline |
| `.callout` | The footer note under a slide |
| `.qa` | The numbered question list |

Two conventions worth keeping:

- **Everything on a slide stays visible.** Fragments reveal a column or a row at
  a time, they never cover up what came before.
- **Each part has an accent colour**, set by `.s-pregnancy`, `.s-birth`,
  `.s-year` or `.s-money` on the section.
