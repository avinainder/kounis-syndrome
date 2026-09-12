# Interventional Cardiology Boards – Mentorship & Study System

This folder is your board-prep home base. It is built around three things that actually
move pass rates: **retrieval practice** (questions before re-reading), **spaced repetition**
(the quiz app schedules misses back at you), and **blueprint-weighted time** (study in
proportion to what the exam tests).

## 1. What the exam tests (ABIM Interventional Cardiology Certification)

Approximate content weighting. Verify against the official blueprint PDF:
https://www.abim.org/media/apib3eza/interventional-cardiology-cert.pdf

| Domain | Approx. weight | What it really means |
|---|---|---|
| Case selection & management | ~25% | Who to treat, how, and when: STEMI/NSTE-ACS pathways, stable CAD, LM/MVD, shock, structural indications |
| Procedural techniques | ~25% | Access, guides, wires, bifurcation, CTO, calcium, SVG, complications and bailouts |
| Basic science | ~15% | Coronary physiology (FFR/iFR/CFR/IMR), hemodynamics, shunts, valve math, restenosis/thrombosis biology, device engineering |
| Pharmacology | ~15% | Antiplatelets, anticoagulants, GPI, vasodilators, contrast, sedation, reversal agents, drug interactions |
| Imaging | ~15% | Angiographic views/anatomy, IVUS, OCT, NIRS, CT for structural planning, echo/TEE guidance |
| Miscellaneous | ~5% | Radiation safety, statistics/trial design, ethics, quality (NCDR, AUC), consent |

Exam format: one day, multiple sessions of single-best-answer questions, many with cine
angiograms, IVUS/OCT frames, hemodynamic tracings, and ECGs. Expect the media questions to be
about **recognition** (dissection grade, perforation class, tracing patterns), so drill images.

## 2. How this folder is organized

```
boards/
  README.md          <- this plan
  progress.md        <- your log; I read this at the start of every session
  quiz.html          <- open in any browser; spaced-repetition question bank (no server needed)
  questions.js       <- the question bank (add questions here; the quiz loads it)
  notes/
    01-coronary-physiology-and-intravascular-imaging.md
    02-pharmacology.md
    03-complications-and-vascular-access.md
    04-hemodynamics-shock-and-mechanical-support.md
    05-structural-heart.md
    06-lesion-subsets-and-revascularization-strategy.md
    07-peripheral-radiation-and-statistics.md
    08-landmark-trials-one-liners.md
```

## 3. The 12-week plan

Assumes ~10–12 focused hours per week. Compress to 8 weeks by merging weeks 9–12 into 2.
Each week: read the note, do the tagged questions in the quiz, and log misses in
`progress.md`. Every miss becomes a one-line "rule" in your own words.

| Week | Focus | Note(s) | Quiz filter |
|---|---|---|---|
| 1 | Coronary physiology, IVUS/OCT | 01 | physiology, imaging |
| 2 | Antithrombotics, contrast, vasoactive drugs | 02 | pharmacology |
| 3 | Complications: perforation, dissection, no-reflow, access | 03 | complications, access |
| 4 | Hemodynamics, shunts, valve math, shock, MCS | 04 | hemodynamics, shock |
| 5 | Structural: TAVR, TEER, BMV, PFO/ASD, LAAO, ASA | 05 | structural |
| 6 | ACS pathways, stable CAD, LM/MVD decisions | 06 | case-selection |
| 7 | Bifurcation, CTO, calcium, SVG, ISR, thrombus | 06 | technique |
| 8 | Peripheral, carotid, PE, radiation, stats | 07 | peripheral, radiation, statistics |
| 9 | Landmark trials sweep; full mixed quiz #1 | 08 | all |
| 10 | Weak-domain rebuild (from progress.md) | as needed | weakest 2 domains |
| 11 | Full mixed quiz #2 + media drill (tracings, angio classifications) | 01, 03, 04 | all |
| 12 | Taper: only "leech" cards (missed ≥2x), rules list, sleep | progress.md | leeches |

Weekly rhythm that works for residents/fellows on service:
- **Mon/Wed/Fri (45 min):** 20–25 questions in the quiz, explanations read closely, misses logged.
- **Tue/Thu (45 min):** read the week's note actively (cover-and-recall, not highlighting).
- **Sat (2–3 h):** long block of mixed questions + write your rules list.
- **Sun:** off, or 15 minutes of leech cards only.

## 4. How I will work with you

- **Socratic first.** When you bring a case or a topic, I will ask what you would do before
  telling you. The exam rewards decision-making, not recall.
- **Blueprint discipline.** If you drift into low-yield rabbit holes, I will pull you back
  to the weighting above.
- **Miss analysis, not miss counting.** For every wrong answer we classify the reason:
  knowledge gap, misread stem, second-guessed a correct first instinct, or a
  distractor trap. Each category has a different fix.
- **Rules in your own words.** By exam day you should have ~150 one-line rules in
  `progress.md`. Rereading those the final week is worth more than any textbook chapter.

## 5. Session starters (paste any of these to me)

- `Quiz me: <domain>` – I will ask board-style vignettes one at a time and grade you.
- `Teach: <topic>` – a focused 10-minute explanation followed by 3 questions.
- `Case: <describe>` – walk through a case as an oral exam.
- `Review my misses` – I read progress.md and rebuild the plan around the weak spots.
- `Tracing drill` / `Angio drill` – rapid recognition practice.

## 6. Bring-your-own resources

Use one question bank in parallel (SCAI / ACC IC SAP, or a commercial IC bank). When a
question there surprises you, add it to `questions.js` in your own words. Building the bank
is itself the best study.

## 7. First assignment

1. Open `quiz.html`, choose **All domains**, and do 40 questions cold as a diagnostic.
2. Record the per-domain score it shows into `progress.md` under "Diagnostic".
3. Tell me your exam date, your weakest two domains from the diagnostic, and how many
   hours per week you can protect. I will then rebuild the 12-week plan around you.
