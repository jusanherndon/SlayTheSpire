# SlayTheSpire

On line 11 of  `SlayTheSpireData.py` insert the path to the directory containing your run history data.
- For Windows this should looks something like `C:\Users\YOUR_NAME\AppData\Roaming\SlayTheSpire2\steam\STRING OF NUMBERS\profile1\saves\history`
- I believe for Mac, the path should begin `~/Library/Application Support/SlayTheSpire2/`

This file build two DataFrames:
  - `df` contains information about every relic for every run
  - `cards_df` contains information about card pick rates

The script will also run some basic data analysis on those DataFrames:
  - A graph of the least successful relics
  - A printout of the most ignored and most picked cards
  - An interactive plot showing card pick rates plotted against win rates


  [Slay the Spire 2 database](https://slaythespire2.gg)

# Quickstart

0. (optional) setup python virtual environment

  a. use UV: https://docs.astral.sh/uv/getting-started/installation/
  b. use venv or builtin python environment


1. install python dependencies
  a. `uv sync`
  b. `pip install .`
  c. `pip3 install .`

2. update save file path in script

Find saves directly in game:
   - Open the game.
   - Press the tilde key (~) to open the console/debug menu.
   - Type open saves and press Enter. This will open the file manager to the exact location. 
   - use `pwd` and copy file path
   - paste path into `folder_path` variable

3. run script

  a. `uv run SlayTheSpireData.py`
  b. `python SlayTheSpireData.py`
  c. `python3 SlayTheSpireData.py`
