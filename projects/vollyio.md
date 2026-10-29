# Vollyio

**Personal project** · July – Aug 2026 · [Live site](https://vollyio.com) · [Public repo](https://github.com/TxaisX/vollyio)

📄 **Full research paper:** [Vollyio: Measuring an AI Skill Grade and a Market, and Closing the Product](vollyio-paper.md) (about 4,400 words)

## What it is

A volleyball skill-analysis app for web and Android. A player uploads a short clip and marks themselves, and a vision model gives a coach's read of their serve, pass, set, attack, block or dig: strengths, one priority fix, and drills.

## What I built

| | |
|---|---|
| Build time | 7 weeks (July 6 – Aug 27, 2026) |
| Commits | 363 |
| Written decisions | 127, each recording what was measured, what it cost, and why |
| Automated tests | 754 |
| Platforms | Web and Android, with working payments and security review |
| Calibration set | 415 labeled clips |

## Why I closed it as a product

I measured whether the grade could be trusted, and it couldn't:

- The model sees about one blurry still per second of video.
- On my own calibration set, the same clip scored differently from run to run (reliability 0.64).
- Beginner and pro footage scored almost the same (81.7 vs 83.5).

I also researched the market. No individual-player grading app had real traction. The volleyball products that succeeded sold match stats and highlights, not technique grades.

So I stopped building, wrote the reasoning down with every number, and kept the site up free as a record.

## What I learned

**Test demand before the second week of building.** One post where players hang out would have answered the question that seven weeks of features couldn't. I apply that now: a cheap test first, the build after.
