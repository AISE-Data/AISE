# Data Dictionary — AISE Occupations (v1)

**File:** `data/occupations/AISE_occupations_v1.csv`  
Each row = one O*NET occupation.

> Note on column names with spaces/symbols: keep them as-is.  
> In Python/pandas use `df['O*NET-SOC Code']`, `df['AISE']`, etc.  
> In R use backticks if needed: `df$`O*NET-SOC Code``.

| Column               | Type   | Description |
|---------------------|--------|-------------|
| O*NET-SOC Code      | string | O*NET-SOC occupation code (e.g., `15-1252.00`). |
| Title               | string | O*NET occupation title (job name). |
| AISE                | float  | **AI Startup Exposure** score computed as in the paper “Follow the money: a startup-based measure of AI exposure across occupations, industries and regions”. Higher = more AI exposure.|
| complementarity     | float  | Complementarity index following **Pizzinelli et al. (2023)** “Labour Market Exposure to AI: Cross-Country Differences and Distributional Implications”. Positive = more complementary to AI|
| job zone            | integer| O*NET **Job Zone** (education/training level). Typically integers 1–5 per O*NET. |
| robotic             | float  | **Robotic Startup Exposure (RSE)** as defined in the supplementary information of “Follow the money: …”. Higher = more exposure to robotics. |

