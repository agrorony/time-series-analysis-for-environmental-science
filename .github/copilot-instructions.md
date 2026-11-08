# Course repository guidance

- Keep explanations and code comments clear, beginner-friendly, and in English.
- Use Python and Jupyter notebooks for teaching examples; use `src/env_timeseries/` for reusable logic rather than duplicating it across notebooks.
- Number notebooks and lessons in learning order. Each notebook should state its learning goals, data source, units, temporal resolution, assumptions, and expected outputs.
- Make examples reproducible: set random seeds where relevant, use explicit paths relative to the repository root, and avoid relying on machine-specific files.
- Preserve raw environmental observations. Document quality-control steps, missing-data handling, time zones, units, and resampling choices before analysis.
- Never add credentials, private data, or large datasets to version control. Keep data acquisition instructions with the relevant lesson.
- Add or update tests for reusable Python code and run `pytest` after code changes.
