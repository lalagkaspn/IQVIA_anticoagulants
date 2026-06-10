# Anticoagulant utilization in Greece, 2018–2022: trends and time-series forecasts

In this work, we aim to quantify national trends in ambulatory anticoagulant consumption in Greece during 2018–2022 and to forecast utilization through 2030 using standardized drug-utilization metrics (Defined Daily Dose/1,000 inhabitants/day). To achieve this, we conduct a retrospective pharmacoepidemiological analysis of national anticoagulant sales data provided by IQVIA Hellas. This data represents community pharmacy sales and we use it as a proxy for population-level drug use. For each anticoauglant drug, we examine drug-specific temporal trends and train SARIMA models to forecast consumption through 2030. Our main conclusion is that anticoagulant utilization in Greece has shifted toward direct oral anticoagulants (DOACs), with concurrent declines in vitamin K antagonists.

In this repository you will find:
- `Anticoagulants_analysis.ipynb`: Jupyter notebook including all analyses and visualizations we did. At the end of the Jupyter notebook, you can find all the libraries we used and their versions.
- `environment.yml`: the accompanying conda environment.
- `sarima_hyperparameter_results.csv`: SARIMA model training results.
-  `sarima_future_forecasts_with_CI.csv`: drug consumption forecasts with 95% confidence intervals. 

The Jupyter notebook requires as input a table where the first column contains month/year entries (e.g., 01/2018) and the following columns contain monthly DDD/1,000 inhabitants/day values (one column per drug). However, we are not permitted to redistribute the IQVIA Hellas data. Therefore, you will not be able to succesfully run the Jupyter notebook. We simply provide it for reference in case you want to see what we did.

If you have any questions, please reach out to [panagiotis.lalagkas@gmail.com](mailto:panagiotis.lalagkas@gmail.com)

## Libraries and Versions

The project was developed and tested with the following package versions:

```text
pyside6==6.9.2
asttokens==3.0.0
comm==0.2.3
contourpy==1.3.3
cycler==0.12.1
debugpy==1.8.16
decorator==5.2.1
et-xmlfile==2.0.0
exceptiongroup==1.3.0
executing==2.2.1
fonttools==4.59.2
importlib-metadata==8.7.0
ipykernel==6.30.1
ipython==9.5.0
ipython-pygments-lexers==1.1.1
jedi==0.19.2
joblib==1.5.2
jupyter-client==8.6.3
jupyter-core==5.8.1
kiwisolver==1.4.9
matplotlib==3.10.6
matplotlib-inline==0.1.7
munkres==1.1.4
nest-asyncio==1.6.0
numpy==2.3.3
openpyxl==3.1.5
packaging==25.0
pandas==2.2.2
parso==0.8.5
patsy==1.0.1
pexpect==4.9.0
pickleshare==0.7.5
pillow==11.3.0
pip==25.2
platformdirs==4.4.0
prompt-toolkit==3.0.52
psutil==7.0.0
ptyprocess==0.7.0
pure-eval==0.2.3
pygments==2.19.2
pyparsing==3.2.3
python-dateutil==2.9.0.post0
pytz==2025.2
pyzmq==27.1.0
scikit-learn==1.7.2
scipy==1.16.1
seaborn==0.13.2
setuptools==80.9.0
shiboken6==6.9.2
six==1.17.0
stack-data==0.6.3
statsmodels==0.14.5
threadpoolctl==3.6.0
tornado==6.5.2
tqdm==4.67.1
traitlets==5.14.3
typing-extensions==4.15.0
tzdata==2025.2
unicodedata2==16.0.0
wcwidth==0.2.13
wheel==0.45.1
zipp==3.23.0
autocommand==2.2.2
backports.tarfile==1.2.0
inflect==7.3.1
jaraco.collections==5.1.0
jaraco.context==5.3.0
jaraco.functools==4.0.1
jaraco.text==3.12.1
more-itertools==10.3.0
tomli==2.0.1
typeguard==4.3.0
```
