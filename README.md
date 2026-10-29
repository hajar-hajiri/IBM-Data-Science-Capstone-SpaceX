# IBM Data Science Capstone — SpaceX Falcon 9

**Repository:** https://github.com/hajar-hajiri/IBM-Data-Science-Capstone-SpaceX

## Project objective
Explore SpaceX Falcon 9 missions and investigate which factors are associated with first-stage landing success. The project is being reconstructed from the IBM course methodology.

## Status (important)
**Work in progress.** The two initial notebooks are original reconstruction exercises, not a claim that all IBM labs have been completed. **No results are claimed until cells are executed.**

## Files
- `notebooks/01_SpaceX_API.ipynb` — retrieves current launch records through the public SpaceX API v4.
- `notebooks/02_Data_Wrangling.ipynb` — audits and transforms those records, exports a simple plot.
- `requirements.txt` — dependencies.
- `data/`, `figures/`, `dashboard/`, `reports/` — intended outputs and next steps.

## Run
1. Install dependencies: `python -m pip install -r requirements.txt`
2. From the **repository root**, start: `jupyter notebook`.
3. Run `notebooks/01_SpaceX_API.ipynb` with **Kernel → Restart & Run All**.
4. Then run `notebooks/02_Data_Wrangling.ipynb`.
5. Commit the notebooks with their executed outputs plus the produced CSV and PNG files, if permitted by course instructions.

## Data sources
- Public SpaceX API v4: https://github.com/r-spacex/SpaceX-API
- IBM capstone course submission requirements: https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/labs/module_5/Submission_Overview_and_Instructions.pdf

## Data limitations
The **current** API is not IBM's fixed historic dataset. Launch counts and success statistics therefore differ from older IBM notebook solutions. `Success` (mission success) and `LandingSuccess` (first-stage landing result) must not be confused. Missing landing statuses are not treated as failure.

## Next steps
Download the historical IBM course datasets, reconstruct remaining labs (scraping, SQL, visual EDA, Folium, Dash, ML), run and save plots/tables, then author a slide deck using **actual outputs**, export PDF, and submit the repository URL.
