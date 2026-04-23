# Antarctic Glacier Analysis

Deep learning pipeline that predicts future Antarctic glacier distributions by learning from historical satellite time-series imagery.

Project period: April 28, 2025 – May 16, 2025

## Data Source

National Snow and Ice Data Center: https://nsidc.org/data/seaice_index/data-and-image-archive

## Layout

```text
.
├── code/                 # Notebooks (data prep, models) and Flask web app archive
├── data/
│   ├── input/
│   │   ├── ice_extent/   # NSIDC ice extent index series
│   │   ├── image_orig/   # Raw imagery (gitignored; fetch from NSIDC)
│   │   ├── image_grey/   # Grayscale conversion (gitignored)
│   │   └── image_resized/# 256x256 resized imagery (gitignored)
│   └── output/           # Model predictions (AE+GRU, ConvLSTM2D, GAN)
├── docs/                 # Planning and final presentations
├── pyproject.toml
└── Makefile
```

## Setup

```bash
make install          # uv sync + install pre-commit
make jupyter          # open Jupyter Lab
```

Raw imagery is not tracked in git. Download the archive from NSIDC into `data/input/image_orig/` before running preprocessing notebooks.

## Features

- Grayscale transformation and 256×256 resizing of satellite image data (1978-11 – 2025-04)
- Moving average, extent distribution, and seasonal decomposition for EDA
- 60-month sequence input with autoregressive 1-month-ahead forecasting
- Flask web app for querying predicted glacier imagery by date

## Models

SARIMAX, CNN, LSTM, Transformer, ConvLSTM2D, AutoEncoder+GRU, U-Net+GAN.

## Conventions

See [REVIEW.md](REVIEW.md) for branch, commit, and PR conventions, and [CONTRIBUTING.md](CONTRIBUTING.md) for the dev loop.

## Contributors

- Choi Hwankyu
- [Park Junho](https://github.com/Moulru)
- Kim Sihwan
- [Kimm Soo Min](https://github.com/somnio-kimm)
