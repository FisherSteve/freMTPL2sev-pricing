# freMTPL2sev - Pricing (Counts)

**Ziel:** Reproduzierbare Notebooks zu Claim-Counts (GLM/GAM/Boosting), korrekt mit `log(Exposure)` als Offset.
**Daten:** Nicht im Repo; siehe `data/README_data.md`. Keine regulatorischen Aussagen.

## Struktur
- `notebooks/`
  - `01_eda_preprocessing.ipynb`
  - `02_glm_gam_boosting.ipynb`
  - `03_novel_model_calibration.ipynb`
- `src/`   Hilfsfunktionen (Datenladen, Metriken, Plots)
- `env/`   Umgebungsdateien
- `data/`  **keine Rohdaten**, nur Hinweise

## Repro (Kurz)
```bash
uv venv --python 3.11 .venv
source .venv/bin/activate
uv pip sync -r env/requirements.txt
jupyter lab

