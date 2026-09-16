# IT3212 Assignment 1

Grupperepository for Assignment 1 i IT3212.

Hoveddatasettet som brukes i oppgaven er:

`smoking_driking_dataset_Ver01.csv`

Datasettet er ikke inkludert i repositoryet på grunn av filstørrelsen. Last det ned fra Canvas og legg det i `data/`-mappen.

Enkleste er nok å laste ned smoking-drinking.zip og og ipynb filen og kjøre i https://jupyter.ntnu.no/ ellers:

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

## Task 2: manglende verdier

Last ned `spanish-cities-energy-consumption.zip` fra kursmaterialet og pakk ut
`energy_dataset.csv` til `data/energy_dataset.csv`. Værfilen i samme arkiv trengs ikke.
CSV-filer og `data/` er allerede utelatt fra Git.

Kjør `src/data-driven.ipynb` med `src/` som arbeidsmappe og prosjektets Python-miljø
som kernel. For å kjøre hele notebooken trengs også smoking/drinking-filen beskrevet
over. Energicellene under «Missing values in a second dataset» kan kjøres separat
ovenfra og ned, og trenger bare `energy_dataset.csv`.

Task 2 viser manglende verdier per kolonne, fjerner to helt tomme kolonner og
interpolerer de resterende 401 manglende verdiene. Begrunnelse, begrensninger og
før/etter-tabell står i notebooken. Eksemplet bruker egne `energy_`-variabler og
endrer ikke hoveddatasettet.


## Prosjektstruktur

```text
assignment-1/
├── data/
│   └── smoking_driking_dataset_Ver01.csv
├── notebooks/
    └── data-driven.ipynb
