# Lecture 3 Rework — Handoff Prompt

Use this document when starting a **separate** pedagogy pass on `Lecture3_lesson.ipynb`. Do not bundle with Lecture 2 edits.

## Context

Day 2 Lecture 2 (`Lecture2_If_statements/Lecture2_lesson.ipynb`) teaches if-statements with geoscience scalar examples before students reach loops. Lecture 3 needs a coordinated pedagogy rework to match the Lecture 1 / Lecture 2 notebook conventions.

## What Lecture 2 teaches (assume before L3)

- `if` / `elif` / `else`, comparison operators, `==` vs `=`
- Geoscience scalar examples: wind speed categories (calm / moderate / strong), season from month number
- `if x in list` membership (including `month in [12, 1, 2]` vs `or` chains)
- Compound conditions: `and` (e.g. `year == 2020 and month == 6`) and `or` in core
- Pair+share green Tasks and predict-before-run pattern
- Afternoon `Lecture2_challenge.ipynb` reinforces wind/season/`in` without loops

## Lecture 3 problems identified

- Overfull for 60–75 min: loop intro + lidar exploration + **20-min code-annotation block** on June 2020 extraction + plot capstone
- Duplicate “what does this tell us” Q&A cells during data exploration
- Previously used `if year_i == 2020 and month_i == 6` without prior `and` teaching — **addressed by L2 §1.6**
- Season definitions (winter = Dec/Jan/Feb) overlap L2 challenge — L3 should **reference** morning work, not re-teach
- Red “refactor loops” task is advanced — candidate for Dive Deeper
- Pedagogy thinner than reworked L1/L2: few predict blocks, no instructor timing callout, no tiered goals

## Requested L3 rework goals

1. Apply same notebook conventions as Lecture 1/2: outcome-based goals, instructor timing (~65 min core), green Tasks, red Dive Deeper, optional in-lesson stretch
2. **Bridge from L2:** “This morning you classified wind speeds and seasons with `if`; now we loop over thousands of lidar records and filter with `if` inside the loop”
3. **Trim core path:** Shorten 20-min annotation to ~5 min instructor walkthrough; move line-by-line notes to optional markdown or Dive Deeper
4. **Do not re-teach:** basic `if`/`elif`, `and`/`or`, season month lists — assume L2 core
5. **Keep in L3 core:** `for` loops, `range(len(arr))`, loop + `if` combination, lidar data load, June 2020 hourly extraction (simplified presentation), one real-data plot
6. **Align** with `Lecture3_challenge.ipynb` seasonal daily-average capstone
7. Phase 1 = lesson only; defer solutions/challenge/README like L1/L2

## Reference files

- Pedagogy model: `Lecture1_Arrays_and_Plotting_2/Lecture1_lesson.ipynb`, `Lecture2_If_statements/Lecture2_lesson.ipynb`
- Original source: `Day 3_Loops and if statements/Day_3_lesson.ipynb`
- Data: `Day2/data/lidar_winds_short.csv`

## Open questions for L3 pass

- How many pair+share tasks in L3 (if any)?
- How much of the June 2020 block should students write vs copy-paste?
- Should L3 get its own `Lecture3_dive_deeper.ipynb` like L1?
