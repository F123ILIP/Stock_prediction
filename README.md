# Stock Prediction (LSTM)

A compact, reproducible project exploring **next-step stock price forecasting** using an **LSTM** baseline. The goal of this repository is to document the end‑to‑end workflow: data preparation, model training, evaluation, and visualization.

> Note: This repository currently links to a Google Colab notebook used to run the experiments. A local setup section is included below (template-style) and can be finalized once the exact file layout is confirmed.

## What’s inside
- Time series preprocessing (windowing / scaling)
- LSTM model training (baseline)
- Evaluation and visual comparison of predictions vs. ground truth
- Example plots included in the README

## Quick start
### Option A — Run in Colab (recommended)
Open the notebook here:
- https://colab.research.google.com/drive/12oHASWtuBfugBthj0p9wiEagW7-eV1hf

### Option B — Run locally (template)
> Adjust commands once you confirm your exact entrypoint (e.g. `train.py`, `main.py`, or a notebook).

1. Create environment
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # macOS/Linux
   .\.venv\Scripts\activate   # Windows
   ```
2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```
3. Run
   ```bash
   python train.py
   ```

## Results (example outputs)
### Historical data
![Historical data](https://github.com/user-attachments/assets/ef5ab629-c91b-4f3c-8909-2faab919c273)

### Model evaluation
![Model evaluation](https://github.com/user-attachments/assets/af0f57f4-0122-4f72-b4cb-9ea6ca9b3c0f)

### 30-day forward prediction
![30-day prediction](https://github.com/user-attachments/assets/33dbf560-309a-47db-9e82-17e52a37b16a)

## Reproducibility checklist
- [ ] Fix random seeds (NumPy / Python / framework)
- [ ] Track dataset version and preprocessing parameters
- [ ] Save model checkpoints + config used for training
- [ ] Keep a single command to reproduce results

## Roadmap
- [ ] Add a clear project structure (`src/`, `notebooks/`, `data/`)
- [ ] Add `requirements.txt` or `environment.yml`
- [ ] Add baseline comparisons (naïve last-value, linear regression, XGBoost)
- [ ] Add proper backtesting (walk-forward validation)

## Credits
Some parts were inspired by Greg Hogg’s tutorial:
- https://youtu.be/CbTU92pbDKw

## License
Choose a license (MIT is a good default). If you want, I can add one.