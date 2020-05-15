# Static source code metrics and static analysis warnings for fine-grained just-in-time defect prediction

This replication kit contains the jupyter notebooks used to aggregate the results of the mining process.

## Download data

This download contains the raw mined data used to generate the evaluation data already contained in this replication kit. You do not need to download this if you only want to re-create the plots and tables.
```bash
cd data
wget https://mediocre.hosting/icsme2020.zip
unzip icsme2020.zip
```

## Install dependencies for jupyter lab

```bash
python -m venv .
source bin/activate
pip install -r requirements.txt
```

## Run jupyter lab

```bash
source bin/activate
cd notebooks
jupyter lab
```

Jupyter lab is used to aggregate the results and create the plots.
To aggregate the data run the TrainTest.ipynb and Interval.ipynb notebooks. Both aggregate the pydriller_*.csv to aggregated results.

The plots are generated by TrainTestEval.ipynb and IntervalEval.ipynb.

Overview.ipynb and Correlation.ipynb provides an overview of the data and the top 10 features.
