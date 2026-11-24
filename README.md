# CRM & CM with Business Intelligence - CWK1 (6BUIS017W)

S&P 500 stock segmentation with adapted RFM (Recency, Frequency, Monetary) measures, using a frozen daily-price snapshot, plus a data mart design and a critical review of the results.

## What is here
- `CRM_CW01_w2052134.ipynb` - the full analysis: Task 1 (data preparation and features), Task 2 (Ward and K-means clustering, sensitivity), Task 3 (data mart, review of results). All outputs and checks are saved in the notebook.
- `data/` - the frozen snapshot (raw prices, `snapshot_info.json` with MD5 fingerprints, retrieval date 19 Nov 2026 10:27 UTC), the Task 1 feature tables, and the Task 2 cluster assignments and comparison tables.
- `data/mart/` - the Task 3 data mart: fact and dimension tables, cluster assignments, run parameters, file lineage and the version register.
- `figures/` - all figures used in the analysis.

## How to re-run
1. Open the notebook in Google Colab (the badge at the top of the notebook).
2. Choose Runtime > Run all. The data is restored from this repository; nothing is downloaded live (`ALLOW_LIVE_DOWNLOAD = False`), so results reproduce the frozen snapshot.
3. The notebook mounts Google Drive by default. To run without Drive, set `USE_GOOGLE_DRIVE = False` in the SETUP cell.
4. Each step prints PASSED lines for its built-in checks.
