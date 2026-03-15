# AI Exposure of the Israeli Job Market

An interactive visualization of AI exposure across **112 Israeli occupations**, covering ~3 million workers.

**[🚀 Live Demo](https://yobens5.github.io/jobs-israel)**

## What it shows

- **Treemap** — Each rectangle is an occupation. Size = employment, colour = AI exposure (green → red, 0–10).
- **Exposure vs Outlook** — Scatter plot comparing AI exposure against 10-year employment outlook.
- Hover any occupation for median pay (₪ NIS), employment, AI score, rationale, and education requirements.

## Key findings

| Stat | Value |
|------|-------|
| Occupations covered | 112 |
| Jobs represented | ~3.0M |
| Weighted avg. AI exposure | **4.9 / 10** |
| Jobs in high-exposure roles (7+) | ~28% |
| Annual NIS payroll at risk | ~₪150B |

Israel's exposure (4.9) is higher than Canada (3.7) due to its large high-tech sector.

## Data sources

| Source | Publisher |
|--------|-----------|
| Labour Force Survey 2022–2023 | Central Bureau of Statistics (CBS) Israel |
| ISCO-08 occupation classification | International Labour Organization |
| Labour market outlook | Israeli Employment Service (Taasuka) |
| AI exposure scores | GPT-4o-mini via OpenAI API |

## Running locally

```bash
cd site && python3 -m http.server 8080
# Open http://localhost:8080
```

## Rebuilding the dataset

```bash
python3 build_site_data_il.py
```

## Credits

- **Original**: [Andrej Karpathy — karpathy/jobs](https://github.com/karpathy/jobs)
- **Israeli adaptation**: ISCO-08 mapping, CBS Israel data, Yohan Bensoussan @yobens5
