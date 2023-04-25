README.md



# Step 1
Configure patches


# Step 2:

Download data from EVG

```sh
./postprocess.sh fetch_ftdc perf1.yml
```

# Step 3:****

Postprocess FTDC into JSON

```sh
./postprocess.sh ftdc_to_json perf1.yml
```

# Notebooks

Open these jupyter notebooks, see https://jupyter.org/
OR use VS Code - https://code.visualstudio.com

notebooks/es_summary_analysis.ipynb
notebooks/es1_analysis.ipynb


====================

To generate perf criteria reports

sh ./postprocess.sh genny_stats perf_criteria_60.yml > perf_criteria_60.csv
sh ./postprocess.sh genny_stats perf_criteria_70.yml > perf_criteria_70.csv

sh ./postprocess.sh genny_stats perf_criteria_60_unencrypted.yml > perf_criteria_60_unencrypted.csv
sh ./postprocess.sh genny_stats perf_criteria_70_unencrypted.yml > perf_criteria_70_unencrypted.csv

sh ./postprocess.sh genny_stats perf_criteria_threads.yml > perf_criteria_threads.csv

sh ./postprocess.sh genny_stats perf_criteria_60_fixed.yml > perf_criteria_60_fixed.csv
