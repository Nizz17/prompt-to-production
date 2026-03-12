# Skills

### 1. `classify_complaint`
- **Input**: A single text description from a citizen.
- **Action**: Uses an LLM to evaluate the text against a strict constraints list.
- **Output**: Returns a dictionary/JSON with exact keys: `category`, `priority`, `reason`, `flag`.

### 2. `batch_classify`
- **Input**: Command Line Arguments for `--input` (CSV) and `--output` (CSV).
- **Action**: Opens the target CSV, iterates row by row, calls `classify_complaint` on the description column, and appends the resulting schema.
- **Output**: Writes the completed rows to `results_[city].csv`.
