# Generative Algorithms Final Project

This repository contains a generative audio analysis and decoding project using neural audio codecs.

## Contents

- `Demo.ipynb` - demo notebook showing full audio processing, encoding, decoding, and feature analysis.
- `requirements.txt` - Python dependencies for running the demo.
- `audio_files/` - source audio samples used by the notebook.
- `ecdc/` - example serialized token files (`.ecdc`) containing encoded audio representations.
- `utils/ecdc_utils.py` - helper utilities for loading audio, converting between token formats, and working with latent audio representations.
- `Documentation.pdf` - additional documentation and project write-up.
- `feature_preservation.png`, `pca_latents.png`, `utilization.png` - result visualizations from the notebook.

## Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage

1. Launch Jupyter Notebook:

```bash
jupyter notebook Demo.ipynb
```

2. Open `Demo.ipynb` and run the cells in order.

3. The notebook performs:
   - loading source audio samples
   - initializing EnCodec and DAC models
   - encoding audio to discrete tokens
   - constructing token-to-latent look-up tables
   - performing progressive decoding at selected codebook levels
   - extracting audio features such as pitch, centroid, flatness, MFCC, and chroma
