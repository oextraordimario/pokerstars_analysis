My idea with this project was to analyse data from my PokerStars matches and find ways to improve my strategy.

It currently has three files, all formatted as Python Notebooks (.ipynb):
- "A-raw_to_json.ipynb" turns all .txt match log files in a folder into their respective .json files with semi-structured data. It uses a lot of regex and, for example, turns "PokerStars Hand #240260121319" into {hand_id: 240260121319}
- "B-json_to_silver.ipynb" loops through all the .json files in a folder and turns them into .csv files. These are structured tables built according to the data model I'd previously designed
- "C-silver_to_gold.ipynb" reads the silver .csv files and applies many transformations to correct and enrich the data, making it ready for analysis.

This was my first real experience building an ETL in Python and using unstructured and semi-structured data. I now realize there are many things I could have done better, but that's what this experience was for!
