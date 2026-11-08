# Time Series Analysis for Environmental Science

Course workspace for learning time-series methods through environmental data. The local course outline and the published 2026/2027 calendar are summarized in [COURSE_GUIDE.md](COURSE_GUIDE.md) and [SCHEDULE_2026-2027.md](SCHEDULE_2026-2027.md). Lessons and notebooks in this repository are intended to be developed for this workspace; datasets should be documented before use.

## Repository layout

- `lessons/` — lesson notes and assignment briefs.
- `notebooks/` — executable notebooks, numbered in learning order.
- `data/raw/` — original inputs; keep large or restricted datasets out of Git.
- `data/processed/` — derived datasets that are small and reproducible.
- `src/env_timeseries/` — reusable Python helpers used by notebooks.
- `tests/` — checks for reusable code.
- `COURSE_GUIDE.md` — locally written topic map and learning goals based on the public course overview.
- `SCHEDULE_2026-2027.md` — concise schedule summary; confirm dates against the official calendar.

## Setup

Requires Python 3.10 or later. From the repository root, create and activate a virtual environment using your preferred Python environment manager, then install the project and development dependencies:

```text
python -m pip install -e ".[dev]"
```

Start JupyterLab with `jupyter lab` and open a notebook under `notebooks/`. If the notebook interface is unavailable, install and register the environment's Jupyter kernel using `ipykernel`.

## Working with data

Keep source data unchanged in `data/raw/` and write derived data to `data/processed/`. Document each dataset's source, units, timezone, temporal resolution, missing-value conventions, and any transformations in the relevant lesson or notebook. Do not commit credentials, private data, or large files; provide reproducible acquisition instructions where needed.

## Course material source

The course overview and schedule are based on the publicly available course pages by Yair Mau. This repository summarizes their structure and links to the sources; it does not copy the site's lesson text or course datasets.

## Tests

Run the test suite with `pytest` from the repository root.
