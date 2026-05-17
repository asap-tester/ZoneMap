# ZoneMap
> Know exactly where your marks are leaking — before the exam does.

![image alt](https://github.com/asap-tester/ZoneMap/blob/162b7956b03e536368ac9680799352f100331997/panel.jpg)
![image alt](https://github.com/asap-tester/ZoneMap/blob/162b7956b03e536368ac9680799352f100331997/info.jpg)
![image alt](https://github.com/asap-tester/ZoneMap/blob/162b7956b03e536368ac9680799352f100331997/data.jpg)

## The Problem
Students approaching high-stakes exams have covered most of their syllabus but don't know where to spend their remaining time. Mock tests reveal gaps after the fact. Nothing maps confidence against marks weight to tell you which topic to study next.

## Who It's For
- CA/CFA/CPA/bar aspirant, 3 weeks from an exam, unsure where to focus
- University student with 12+ topics and 10 days left
- Any aspirant who has "studied everything" but feels uneven

## What It Does
- Ranks every topic by risk score (low confidence × high marks weight)
- Colour-codes topics into RED / AMBER / YELLOW / GREEN priority zones
- Shows total marks at risk so you know the stakes of each study session

## How to Use
1. Download `index.html` or copy the raw file
2. Open in any browser — no install, no login, no internet required after first load
3. Add your subject's topics with marks weight and confidence rating — priority map builds instantly

## Deploy to GitHub Pages
1. Create a new GitHub repo (e.g. `zonemap`)
2. Upload `index.html` as the only file in the root
3. Go to **Settings → Pages → Source: main branch → / (root)**
4. Your app is live at `https://[username].github.io/zonemap`

## Priority Score Formula
```
Priority Score = (6 - confidence) × marks_weight
```

| Score | Zone | Action |
|-------|------|--------|
| ≥ 20 | 🔴 RED | Study immediately |
| 10–19 | 🟠 AMBER | Revisit soon |
| 5–9 | 🟡 YELLOW | Schedule review |
| < 5 | 🟢 GREEN | Maintain only |

## Tech
- Vanilla HTML/CSS/JS — zero dependencies
- localStorage for automatic persistence
- Fully offline after first load
- Single file — deploy anywhere

## Roadmap
- [ ] Multi-subject support (switch between exam papers)
- [ ] Revision session planner based on priority map
- [ ] Time-to-exam countdown with daily topic targets
- [ ] WebView wrapper for Play Store / App Store

## License
MIT
