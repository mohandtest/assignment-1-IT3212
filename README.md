# IT3212 Assignment 1

Grupperepository for Assignment 1 i IT3212.

Hoveddatasettet som brukes i oppgaven er:

`smoking_driking_dataset_Ver01.csv`

Datasettet er ikke inkludert i repositoryet på grunn av filstørrelsen. Last det ned fra Canvas og legg det i `data/`-mappen.


## Oppsett:
1. lag en mappe som heter data
2. unzip datasettet smoking_drinking.zip og legg den inn i data
3. for å sette å pythonmiljøet:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

(om du bruker uv i stedet)
```bash
uv sync
```
velg: .venv/bin/python som Jupyter-kernel

For vs-code trenger du nok python og Jupyter extensions

så kan du kjøre src/data-driven.ipynb


## Prosjektstruktur

```text
assignment-1/
├── data/
│   └── smoking_driking_dataset_Ver01.csv
├── notebooks/
    └── data-driven.ipynb
