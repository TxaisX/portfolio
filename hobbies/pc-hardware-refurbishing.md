# PC hardware refurbishing

**Hobby** · Sacramento · Sept 2026 – present

📄 **Full research paper:** [Buying Used PCs by the Numbers: A Deal Tracker and a Five-Report Market Study](pc-hardware-refurbishing-paper.md) (about 4,400 words)

I buy used gaming PCs and parts locally, test and refurbish them, and resell them whole or as parts. Before buying anything, I treated it like any research project: learn the market, write the rules, and build the tracker.

## The tracker

- **Parts database:** 127 GPU and CPU models with tier, performance class, and used-market price.
- **Deal sheet:** each local listing gets a row and a verdict of BUY, NEGOTIATE or PASS, computed from the parts it contains against my price rules. 184 listings tracked.
- **Live dashboard:** a local web page that reads the spreadsheet and redraws a few seconds after each save.
- **Buying rules I set:** GPU floor of an RTX 3080 (30-series) or equivalent; CPU floor of Intel 12th gen or Ryzen 5000; avoid paying market price for single parts; sell RAM within weeks instead of holding it.

## The research

Five research reports ran in parallel on CPUs, GPUs, platforms, the resale market, and testing. Every claim carries an evidence tag:

| Tag | Meaning |
|---|---|
| HARD | Named primary source (manufacturer, benchmark site, sales data) |
| VENDOR | Commercial blog or price aggregator |
| CHARACTERISTIC | Community consensus |
| ESTIMATE | Inference |

I then checked the reports against each other, corrected the errors I found (a misnamed CPU, a duplicated benchmark row, a GPU placed in the wrong tier), and wrote one synthesis.

**Main findings (Sept 2026):**

| Shift | What it means for a reseller |
|---|---|
| RAM and SSD prices roughly tripled to quintupled in a year (AI datacenters buying capacity) | Memory and storage inside a used PC are worth real money. Price them as line items. |
| Used GPUs hold or gain value; some used RTX 50 cards sell above retail | GPUs are the easiest thing to resell |
| Windows 10 support ended Oct 2025 | A flood of old office PCs; only 8th-gen Intel / Ryzen 2000 and newer can run Windows 11 |
| Most buyers spend under $800 | Build and price for the $450–850 range first |

**One data lesson:** "used price" means *asking* price on some sites and *sold* price on others. On an RTX 3090 the gap was about $350. Every price in my tracker says which one it is.

## Bottlenecks, in one idea

The CPU prepares each frame, and that work doesn't change with resolution. The GPU paints it, and that work grows with pixels. At 1080p a weak CPU becomes the limit; at 4K almost any modern CPU keeps up. So "do these parts pair well" always means *at the resolution the buyer plays at*.
