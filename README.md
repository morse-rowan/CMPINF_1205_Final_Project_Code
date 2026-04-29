# AI, Satellite Imagery, and the Emerging Limits of Digital Privacy

**Rowan Morse** · CMPINF 1205: Comparative Digital Privacies · Spring 2026

This repository contains the code and visualizations for my final project. It
combines a zero-shot text-to-patch retrieval demo over overhead imagery
(RemoteCLIP) with a privacy-risk framework and a threshold visualization that
maps current and near-term satellite systems onto a resolution × revisit plane.

## Contents

- `remoteclip.ipynb` — end-to-end notebook
  - **Part 1:** Satellite Privacy Risk Index applied to three reference systems
  - **Part 2:** Privacy threshold visualization
  - **Part 3:** RemoteCLIP retrieval demo 

## Running the notebook

The retrieval demo (Part 3) requires a GPU. Parts 1 and 2 are
matplotlib-only and run anywhere.

### With a GPU (recommended) — Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AFyaVVhGgNXAyEcXgDo-N7P64LJynOsu?usp=sharing)

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. **Runtime → Change runtime type → T4 GPU**.
3. **Runtime → Run all**, then upload an overhead image when prompted at cell 4.
4. Edit the `QUERY` and `TOP_K` parameters in cell 7 and re-run that cell to
   try different queries.

### Without a GPU — Parts 1 & 2 

Parts 1 and 2 are independent of RemoteCLIP and can be run locally without a
GPU. The minimal dependency is matplotlib:


## Sources

- Denis, N. & Di Pietro, R. (2025). *The looming privacy challenges posed by commercial satellite imaging.* IEEE Access, 13, 122432–122444.
- Liu, F. et al. (2024). *RemoteCLIP: A vision language foundation model for remote sensing.* arXiv:2306.11029.
- McAmis, R. et al. (2024). *Over fences and into yards: Privacy threats and concerns of commercial satellites.* PoPETs.
- Planet Labs (2025). *Planet Releases First Light Image From Pelican-6.* Business Wire.
- Copernicus Data Space Ecosystem. *Sentinel-2.*
- ESA Earth Online. *WorldView-3.*
