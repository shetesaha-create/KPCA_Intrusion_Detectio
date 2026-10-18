# ML Algorithms — Kernel PCA Experiments

This repository organizes the 75 Python programs supplied for five algorithms. The Python code was taken from the uploaded source archives / combined SVM source; the code bodies were not rewritten. For the four archive-based groups, only folder and filename organization may differ from the source archive. The combined SVM file was split at its 15 repeated program starts so each program can be stored separately.

## Algorithms

- `01_Elastic_Net/` — 15 programs
- `02_XGBoost/` — 15 programs
- `03_AdaBoost/` — 15 programs
- `04_Support_Vector_Machine/` — 15 programs
- `05_Multilayer_Perceptron/` — 15 programs

Each group is intended to cover five Kernel PCA kernels (RBF, Linear, Polynomial, Sigmoid, Cosine) and test sizes 0.2, 0.4, and 0.6. Filenames are descriptive labels; consult each script's own contents to confirm its exact settings.

## Other supplied materials

- `reference_documents/` — the 15 uploaded Word documents, copied without editing.
- `project_data/py project.xlsx` — the uploaded workbook, copied without editing.
- `source_notes/` — the five original Markdown files, the original combined SVM source, and backups of the four uploaded code archives.

## Dataset requirements

The scripts reference CIC-IDS CSV files such as `Tuesday-WorkingHours.pcap_ISCX.csv`, `Wednesday-workingHours.pcap_ISCX.csv`, and `Thursday-WorkingHours-Morning-WebAttacks.csv`. Those CSV datasets are not included here; place the required dataset files in the working directory before running the scripts.

## Important note

The code bodies are preserved from the supplied `.py` sources/archives, rather than regenerated from the earlier Markdown snippets. This organization does not guarantee that all scripts run in every environment; install the dependencies used by the scripts and check dataset paths first.
