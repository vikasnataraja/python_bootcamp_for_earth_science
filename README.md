# ATOC Python Bootcamp for Earth Science

A short, hands-on **Python bootcamp** for atmospheric, oceanic, and Earth science students. Over five days you move from core Python and plotting into the packages used most often in research workflows: NumPy, Matplotlib, pandas, xarray, and Cartopy.

Materials are Jupyter notebooks with guided lessons, optional challenges, and solution keys.

## Background

This curriculum grew out of the University of Colorado Boulder Department of Atmospheric and Oceanic Sciences (ATOC) **Research Experience for Undergraduates (REU) in Data Science** bootcamp (started 2021). It has since been reworked into a standalone **5-day, 3-lectures-per-day** course that can be used for REU cohorts or other ATOC / Earth science teaching.

The project has always been a department-wide effort. Because notebooks were edited both with and without GitHub, **commits are not a reliable measure of contribution**. Contributors (alphabetical):

- Nathan Agarwal
- Becca Baiman
- Genevieve Clow
- Devon Dunmire
- Tina Geller
- Kara Hartig
- Sean Leister
- Jed Lenetsky
- Michelle Maclennan
- Andrew Metz
- Sam Mogen
- Ethan Murray
- Vikas Nataraja
- Cole Persch
- Clairy Reiher
- Alex Rybchuk
- Megan Thompson-Munson
- Brianna Undzis
- Mikell Warms
- Matt Watwood
- Chris Wyburn-Powell
- Ziqi Yin

## Course structure (5 days)

Each day has up to three lectures. Shared data lives in [`Datasets/`](Datasets/). Student notebooks are under each day’s `Lecture_*` folders; answer keys are in that day’s `Solutions/` folder.

Earlier 9–10 day REU materials are archived under [`Old/`](Old/) for reference (notebooks and docs only; no data files).

### Day 1 — Intro to Python
- Lecture 1: Intro to coding — [`Day_1_Intro_to_Python/Lecture_1_coding/`](Day_1_Intro_to_Python/Lecture_1_coding/)
- Lecture 2: Variables, data types, functions — [`Day_1_Intro_to_Python/Lecture_2_variables_data_types_functions/`](Day_1_Intro_to_Python/Lecture_2_variables_data_types_functions/)
- Lecture 3: Lists + Plotting 1 — [`Day_1_Intro_to_Python/Lecture_3_lists_plotting_1/`](Day_1_Intro_to_Python/Lecture_3_lists_plotting_1/)
- LectureX (alternate, fuller Lists + Plotting 1) — [`Day_1_Intro_to_Python/LectureX_Lists_Plotting1/`](Day_1_Intro_to_Python/LectureX_Lists_Plotting1/)

### Day 2 — Logic and Plotting
- Lecture 1: Arrays + Plotting 2 — [`Day_2_Logic_and_Plotting/Lecture_1_Arrays_and_Plotting_2/`](Day_2_Logic_and_Plotting/Lecture_1_Arrays_and_Plotting_2/)
- Lecture 2: If-statements — [`Day_2_Logic_and_Plotting/Lecture_2_If_statements/`](Day_2_Logic_and_Plotting/Lecture_2_If_statements/)
- Lecture 3: Loops — [`Day_2_Logic_and_Plotting/Lecture_3_Loops/`](Day_2_Logic_and_Plotting/Lecture_3_Loops/)

### Day 3 — Science Packages Pt1
- Lecture 1: Time series (pandas) 1 — [`Day_3_Science_Packages_Pt1/Lecture_1_pandas_1/`](Day_3_Science_Packages_Pt1/Lecture_1_pandas_1/)
- Lecture 2: Time series (pandas) 2 — [`Day_3_Science_Packages_Pt1/Lecture_2_pandas_2/`](Day_3_Science_Packages_Pt1/Lecture_2_pandas_2/)
- Lecture 3: Multi-dimensional arrays (xarray) 1 — [`Day_3_Science_Packages_Pt1/Lecture_3_xarray_1/`](Day_3_Science_Packages_Pt1/Lecture_3_xarray_1/)

### Day 4 — Science Packages Pt2
- Lecture 1: Multi-dimensional arrays (xarray) 2 — [`Day_4_Science_Packages_Pt2/Lecture_1_xarray_2/`](Day_4_Science_Packages_Pt2/Lecture_1_xarray_2/)
- Lecture 2: Geospatial plots (cartopy) 1 — [`Day_4_Science_Packages_Pt2/Lecture_2_cartopy_1/`](Day_4_Science_Packages_Pt2/Lecture_2_cartopy_1/)
- Lecture 3: Geospatial plots (cartopy) 2 — [`Day_4_Science_Packages_Pt2/Lecture_3_cartopy_2/`](Day_4_Science_Packages_Pt2/Lecture_3_cartopy_2/)

### Day 5 — Extras
Flexible wrap-up: data exploration, student-requested special topics, and tooling (git, environments, coding with AI). See [`Day_5_Extras/README.md`](Day_5_Extras/README.md).

## How to use these notebooks

### Environment
Use the conda environment defined in [`reu_env.yml`](reu_env.yml) (name retained from the REU materials).

### Data paths
Notebooks that load files set this in the first code cell:

```python
DATA_FOLDER = "../../Datasets/"
```

Example:

```python
pd.read_csv(DATA_FOLDER + "boco_air_temp.csv")
```

### Notebook colors
- **Teal** (`#0F766E`) — required student tasks
- **Red** (`#B91C1C`) — optional challenges / dive deeper

Use HTML `<font color="#0F766E">...</font>` so colors render in Google Colab as well as local Jupyter.

### Figures
Static lesson images live in [`Figures/`](Figures/) at the repo root (same pattern as [`Datasets/`](Datasets/)). Notebooks set `FIGURES_FOLDER` next to `DATA_FOLDER`:

```python
# Google Colab (after Drive mount)
FIGURES_FOLDER = "/content/drive/MyDrive/python_bootcamp/python_bootcamp_for_earth_science/Figures/"

# Local Jupyter
FIGURES_FOLDER = "../../Figures/"
```

Example:

```python
from IPython.display import Image, display
display(Image(FIGURES_FOLDER + "lidar_array_structure.png"))
```

### File naming
```text
Datasets/                         # shared data files
Figures/                          # shared static lesson images
Day_N_<big_topic>/
  Lecture_K_<mini_topic>/
    DN_Lesson_K.ipynb
    DN_Challenge_K.ipynb          # optional
    DN_Dive_Deeper_K.ipynb        # optional
  Solutions/
    DN_Lesson_K_solutions.ipynb
    DN_Challenge_K_solutions.ipynb
```
