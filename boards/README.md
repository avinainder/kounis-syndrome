# Interventional Cardiology Boards – Mentorship & Study System

This folder is your board-prep home base. It is built around three things that actually
move pass rates: **retrieval practice** (questions before re-reading), **spaced repetition**
(the quiz app schedules misses back at you), and **blueprint-weighted time** (study in
proportion to what the exam tests).

## 1. What the exam tests (ABIM Interventional Cardiology Certification)

Blueprint effective January 2026 (from the official blueprint PDF and exam page, captured Sept 2026).

| Category | Weight | Subcategories | Where to study |
|---|---|---|---|
| Case selection and management | 20% | Chronic ischemic heart disease 6%; UA/NSTEMI 4%; STEMI 6%; STEMI complications 4% | Note 06, Note 04 (mechanical complications), Review §7–8 |
| Procedural techniques | 20% | Planning and execution 5%; lesion subsets 6%; selection and use of equipment 6%; technical troubleshooting 3% | Note 06, Note 01 (imaging-guided optimization), Review §7, §9 |
| Catheter-based management of noncoronary disease | 13% | Structural and valvular case selection 6%; noncardiac vascular 5%; hemodynamics 2% | Notes 05, 07, 04; Review §11–13 |
| Pharmacology | 12% | General 3%; IV antiplatelets 2%; oral antiplatelets 2%; IV anticoagulants 2%; oral anticoagulants <2%; contrast 2% | Note 02, Review §1, §3 |
| Cardiac imaging and assessment | 9% | Diagnostic coronary imaging 5%; general tests 2%; x-ray radiography 2% | Note 01, Note 07 (radiation), Review §6, §2 |
| Complications of coronary intervention | 8% | Cardiac 5%; noncardiac 3% | Note 03, Review §10, §4 |
| Basic science | 6% | Vascular biology 4%; physiology 2% | Review §5, Note 01 |
| Anatomy, variants, pathology | 6% | Cardiac 5%; extracardiac <2% | Note 01 (anatomy section), Review §5 (anomalies), §13 (catheter selection, venous anatomy) |
| Miscellaneous | 6% | Procedure-related data 3%; quality and appropriateness 2%; ethical/legal <2% | Note 07 (statistics, quality), Review §14, §7 (AUC, NCDR) |

How to read it: coronary content (case selection + technique + complications) is 48% of the exam.
Structural and valvular case selection is only 6% and hemodynamics 2%, so a structural fellow
should bank those points quickly and spend the marginal hour on coronary decision-making. Basic
science, anatomy and miscellaneous are 18% combined, are finite, and are the cheapest points on
the exam.

**Format.** Up to 220 single-best-answer questions, about 35 of them unscored pretest items, in four
sessions across roughly a 10-hour day. Media (cine, IVUS/OCT, tracings, ECG) is common. Pacing:
about 55 questions per 2-hour session leaves ~2 minutes per question; flag and move.

**2026 administration.** Exam Oct 6, 2026 (accommodation window Oct 26–30). Registration closed
Jun 28, 2026. Fee $2,995; late fee $400; international center $500. Training, including vacation,
must be complete by Oct 31, 2026. Cancellation refunds: 70% if ≥2 days before, 55% after that, 85%
if the application is disapproved; no-shows forfeit the fee; cancel only in the Physician Portal.
**2027 administration.** Exam Oct 14, 2027; registration Dec 1, 2026 – Jun 15, 2027; late Jun 16–28.

## 2. How this folder is organized

```
boards/
  README.md          <- this plan
  blueprint.md       <- the official Jan 2026 blueprint as a tick-box topic checklist
  progress.md        <- your log; I read this at the start of every session
  quiz.html          <- open in any browser; spaced-repetition question bank (no server needed)
                        hosted copy: https://claude.ai/code/artifact/f9fb5471-06b3-4cd3-b478-5fc3c1a09298
                        (append ?mode=diagnostic for the 80-question cold start)
  questions.js       <- the question bank (add questions here; the quiz loads it)
  notes/
    00-high-yield-review-2026.md   <- your 33-page review, converted and cleaned (read this first)
    01-coronary-physiology-and-intravascular-imaging.md
    02-pharmacology.md
    03-complications-and-vascular-access.md
    04-hemodynamics-shock-and-mechanical-support.md
    05-structural-heart.md
    06-lesion-subsets-and-revascularization-strategy.md
    07-peripheral-radiation-and-statistics.md
    08-landmark-trials-one-liners.md
    09-blueprint-gap-topics.md     <- perioperative evaluation, local anesthetics, contrast physics, imaging chain, cost-effectiveness, device surveillance, consent/documentation, aortic disease
```

## 3. The plan

### 3a. 23-day sprint for the Oct 6, 2026 exam (Sept 13 → Oct 6)

Assumes 2–3 focused hours on weekdays and 5–6 on weekend days. Every day: questions first, reading
second, and 20 minutes turning misses into one-line rules in `progress.md`. Emails: six questions
at 5:30 AM Eastern, answers at 5:45 AM; reply with the block-report form. Use the quiz in
"Due for review" mode so misses cycle back at 1, 3 and 7 days.

| Dates | Block (blueprint share) | Read | Questions |
|---|---|---|---|
| Sep 13–14 (Sun–Mon) | Diagnostic: 80 mixed questions cold; read the review's "What changed" table twice | Review pp 1–3 | All domains, 80 |
| Sep 15–17 | Case selection (20%): chronic IHD, NSTE-ACS timing, STEMI reperfusion, STEMI complications | Note 06; Review §7–8 | case-selection, hemodynamics |
| Sep 18–20 | Procedural technique (20%): bifurcation, CTO, calcium, SVG, ISR, equipment, troubleshooting | Note 06 (technique half); Review §9 | technique |
| Sep 21 (Sun) | Complications (8%) + long mixed block | Note 03; Review §10, §4 | complications + 60 mixed |
| Sep 22–23 | Pharmacology (12%): every table in Note 02 from memory; contrast; sedation; reversal | Note 02; Review §1, §3 | pharmacology |
| Sep 24–25 | Imaging and physiology (9%) + radiation (part of imaging): FFR pitfalls, IVUS/OCT, views | Note 01; Note 07 radiation; Review §6, §2 | physiology, imaging, radiation |
| Sep 26–27 | Noncoronary (13%): structural case selection, peripheral/carotid/renal/PE, hemodynamic calculations | Notes 05, 07, 04; Review §11–13 | structural, peripheral, hemodynamics |
| Sep 28 (Mon) | Basic science + anatomy (12%): plaque biology, remodeling, MI definitions, anomalies, catheter selection, venous anatomy | Review §5, §13; Note 01 anatomy; Note 09 basic-science section | physiology, anatomy |
| Sep 29–30 | Miscellaneous (6%) and blueprint gap topics: statistics, cost-effectiveness, AUC, NCDR, device reporting, consent, perioperative evaluation, local anesthetics; then weakest two domains from progress.md | Note 09; Note 07; Review §14 | statistics + weakest domains |
| Oct 1–3 | Full mixed sets (60/day), leeches only on Oct 3; walk `blueprint.md` and tick every topic you can answer cold, then read only the unticked ones; tracing and angiographic classification drill (NHLBI, Ellis, Medina, Rentrop, TIMI) | progress.md rules list | all, then leeches |
| Oct 4 (Sun) | Timed simulation: two 55-question sessions with a break, exam pacing | none | random, 110 |
| Oct 5 | Rules list only, 60 minutes. Confirm Pearson VUE appointment, ID, route. Sleep. | progress.md | none |
| Oct 6 | Exam | | |

Rules of the sprint: no new sources after Sep 28; the review document and these notes are the
whole universe. Anything you miss twice becomes a written rule. Do not reread chapters; re-answer
questions.

### 3b. 12-week plan for a 2027 sitting (or for a later start)

| Week | Focus | Note(s) | Quiz filter |
|---|---|---|---|
| 1 | Coronary physiology, IVUS/OCT | 01 | physiology, imaging |
| 2 | Antithrombotics, contrast, vasoactive drugs | 02 | pharmacology |
| 3 | Complications: perforation, dissection, no-reflow, access | 03 | complications |
| 4 | Hemodynamics, shunts, valve math, shock, MCS | 04 | hemodynamics |
| 5 | Noncoronary I: TAVR, TEER, BMV, PFO/ASD, LAAO, ASA | 05 | structural |
| 6 | ACS pathways, stable CAD, LM/MVD decisions | 06 | case-selection |
| 7 | Bifurcation, CTO, calcium, SVG, ISR, thrombus | 06 | technique |
| 8 | Noncoronary II: peripheral, carotid, renal, PE; radiation, stats | 07 | peripheral, radiation, statistics |
| 9 | Landmark trials sweep; full mixed quiz #1 | 08 | all |
| 10 | Weak-domain rebuild (from progress.md) | as needed | weakest 2 domains |
| 11 | Full mixed quiz #2 + media drill | 01, 03, 04 | all |
| 12 | Taper: leeches only, rules list, sleep | progress.md | leeches |

Weekly rhythm for the long plan: Mon/Wed/Fri 20–25 questions; Tue/Thu active reading; Sat a
2–3 h mixed block plus rules; Sun off or 15 minutes of leeches.

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

## 7. First assignment (today)

1. Open `quiz.html`, choose **All domains**, count 80, and do them cold as a diagnostic.
2. Copy the per-domain table into `progress.md` under "Diagnostic".
3. Send me the table and your eight diagnostic answers from the chat. I will mark the weakest
   two domains and adjust the Sep 29–30 block.
