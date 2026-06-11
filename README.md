# music21-guides

A beginner-friendly Quick Start guide for [music21](https://www.music21.org/), a Python
toolkit for analyzing, searching, and transforming digital sheet music.

[![Open in nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/ccho-mongodb/music21-guides/blob/main/Learn_Music21.ipynb)

By the end of this guide, you will be able to:

- Install and import music21 into a Python environment
- Create and visualize notes and chords as sheet music
- Apply key and time signatures to a musical sequence
- Play back a musical sequence as MIDI in Jupyter
- Analyze chord progressions using Roman numeral notation

## Prerequisites

- Python 3.8+
- [MuseScore](https://musescore.org/) (required for sheet music rendering via `show()`)

> **Note:** music21's `show()` method renders sheet music as an image using an external
> notation program. MuseScore is free and works on macOS, Windows, and Linux.
> Without it, `show()` raises an error. MIDI playback via `show('midi')` works
> in Jupyter without MuseScore.

## Setup

1. In your terminal, clone the repo:
   ```bash
   git clone https://github.com/ccho-mongodb/music21-guides.git
   cd music21-guides
   ```

2. In your terminal, install dependencies:
   ```bash
   pip install music21 jupyter
   ```

3. Install [MuseScore](https://musescore.org/en/download) for sheet music rendering.

4. In your terminal, open the notebook:
   ```bash
   jupyter notebook Learn_Music21.ipynb
   ```

5. In a notebook cell, configure music21 to find MuseScore:
   ```python
   from music21 import environment
   environment.set('musicxmlPath', '/path/to/mscore')  # update to your install path
   ```

## Notebook contents

| Section | What you'll learn |
| :-- | :-- |
| Install the music21 package | Install via pip |
| Import the package | Wildcard import pattern |
| Add notes to a staff | `Stream`, `Note`, and `show()` |
| Add a chord to a staff | `Chord` objects |
| Set key and time signatures | `Key`, `KeySignature`, `TimeSignature` |
| Play back your music | `show('midi')` in Jupyter |
| Analyze your music | `romanNumeralFromChord()` |

## Related

- [abcjs-demo](https://github.com/ya8282/abcjs-demo) — browser-based ABC notation rendering

## Further reading

- [music21 documentation](https://www.music21.org/music21docs/)
- [music21 YouTube playlist](https://www.youtube.com/watch?v=HBhYWPgxFyg&list=PLHgxFmSNqAetHdPNUxG9MJt7JCMZ-xdwn)
