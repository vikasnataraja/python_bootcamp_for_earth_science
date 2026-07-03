# Day 2: Arrays, Plotting, If-Statements, and Loops

Day 2 builds on Day 1 foundations (variables, functions, lists, and basic plotting) and introduces NumPy arrays, matplotlib, if-statements, and for-loops using geoscience data. 

## Lecture Schedule

| Lecture | Folder | Topics |
|---------|--------|--------|
| 1 | `Lecture1_Arrays_and_Plotting_2/` | NumPy arrays, array manipulation, matplotlib (1D, 2D, histograms) |
| 2 | `Lecture2_If_statements/` | `if` / `elif` / `else`, comparison operators, `in` membership, `and` / `or`, wind & season examples |
| 3 | `Lecture3_Loops/` | For-loops, loops + if on lidar wind data, hourly aggregation capstone |

## Folder Contents

Each lecture subfolder contains:

- `LectureN_lesson.ipynb` — student notebook with activities to complete
- `LectureN_lesson_solutions.ipynb` — answer key
- `LectureN_challenge.ipynb` — independent practice
- `LectureN_challenge_solutions.ipynb` — challenge answer key
- `LectureN_dive_deeper.ipynb` — optional exercises (doc links + mini-challenges; not meant to be covered in the live lecture but maybe useful as references later) 

## Data Files

Shared data lives in `data/`:

| File | Description | Used in |
|------|-------------|---------|
| `boulderdaily.complete.txt` | Daily mean air temperature for Boulder, CO | Lecture 1 challenge |
| `lidar_winds_short.csv` | 10-minute lidar wind speed measurements (subset) | Lecture 3 lesson and challenge |
| `boco_air_temp.csv` | Monthly mean air temperature for Boulder, CO | Lecture0 staging folder only (Day 1 merge pending) |

Notebooks should reference these via `../data/<filename>` from within a lecture subfolder.

## Prerequisites

Students should have completed Day 1, including:

- Variables, data types, and functions
- Lists and basic indexing
- Importing packages
- Basic `plt.plot()` with CSV data

Day 1's guess-the-number challenge provides an optional preview of loops and if-statements; Day 2 Lectures 2–3 cover those topics formally.
