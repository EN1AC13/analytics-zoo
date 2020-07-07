# AutoML for time series forecasting
In this notebook, we use automl to do time series forecasting on NYC taxi dataset.

## Environment
* Python 3.6
* Apache Spark 2.4.3
* Jupyter Notebook
* Matplotlib

## Install Analytics Zoo AutoML
1. Create conda environment.
    1. Install [Conda](https://docs.conda.io/projects/conda/en/latest/commands/install.html).
    2. Create a new conda environment (with name "zoo_automl" for example).
    ```bash
    conda create -n zoo_automl python=3.6
    source activate zoo_automl
    ```
2. Install.
    ```bash
    pip install analytics-zoo[automl]
    ```
    Note that the extra dependencies (including `ray`, `psutil`, `aiohttp`, `setproctitle`, `scikit-learn`,`featuretools`, `tensorflow`, `pandas`, `requests`) will be installed by specifying `[automl]`.


## Run Jupyter after pip install
* install jupyter by `conda install jupyter`
* Run `export ANALYTICS_ZOO_HOME="path to analytics-zoo"`.
* Run `$ANALYTICS_ZOO_HOME/dist/bin/data/NAB/nyc_taxi/get_nyc_taxi.sh` to download the dataset. (It can also be downloaded from its [github](https://raw.githubusercontent.com/numenta/NAB/master/data/realKnownCause/nyc_taxi.csv)).
