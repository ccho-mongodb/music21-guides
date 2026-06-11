# Contributing to music21-guides

Contributions that improve the guide — better explanations, additional examples,
or corrections — are welcome.

## Local Setup

1. In your terminal, clone the repo and install dependencies:
   ```bash
   git clone https://github.com/ccho-mongodb/music21-guides.git
   cd music21-guides
   pip install music21 jupyter
   ```

2. Install [MuseScore](https://musescore.org/en/download) for sheet music rendering.

3. In your terminal, open the notebook:
   ```bash
   jupyter notebook Learn_Music21.ipynb
   ```

> [!TIP]
> Keep code cells runnable top-to-bottom with a fresh kernel.
> Test that `show()` renders correctly and `show('midi')` produces a playback widget.
> Match the existing explanation style: brief context, then code, then output.

## Submitting Changes

1. Fork the repo and create a branch: `git checkout -b your-feature`
2. Make your changes and verify the notebook runs cleanly.
3. Open a pull request with a short description of what changed and why.
