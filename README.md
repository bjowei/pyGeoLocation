# pyGeoLocation

Denne jupyter notebooken leser datasettet fra https://data.norge.no/datasets/d1669dac-f1a3-446e-a94f-4febd79c8e28 og transformerer dei til drupal8 format for import.

## Installasjon

For å køyre denne notebooken trenger du jupyter på din PC. Eg anbefaler at ein installerer følgande program:

- Visual Studio Code (link: https://code.visualstudio.com/)
- Anaconda (link: https://www.anaconda.com/products/individual)

### Visual Studio Code

I Visual Studio Code anbefalar eg å installere følgande extensions:

- Python
- Rainbow csv

Python extensionen lar deg redigere og køyre jupyter notebooks i visual studio code istadenfor å hoste ein anaconda økt og opne den i nettlesaren.

### Anaconda og anacondamiljø

Python-koden i notebooken krever ein del bibiliotek, t.d scipy, numpy, pandas, faker osv. For å kjapt installere dette på din PC og for å håndtere bibiliotek på ein god
måte er det anbefalt å bruke anaconda. 

Aktiver anaconda miljøet i vscode og opne terminalen i rot mappa med miljøet aktivert. (oppsett: https://code.visualstudio.com/docs/python/environments)

For å importere anacondamiljøet køyr kommandoen: `conda env create -f pydigdir.yml`

Då er alle bibiliotek som ein treng for å køyre denne notebooken (og dei andre jupyter notebookane laga på DigDirCamp).

### Litt om jupyter notebook

Ein jupyter notebook består av blokker som kan vere tekst eller kode. Det er vanleg praksis å legge små blokker med kode etter kvarandre med forklarande tekst.
Dette gjer at koden i cellene bygger på kvarandre og ein er nøydd å køyre koden frå topp til bunn (vs code har ein eigen knapp for å gjere dette automatisk)

## Algoritmen

Denne algoritmen gjer ikkje noko meir avansert enn å hente ut dei kolonnene frå datasettet i CSV format som me er interesserte i. Denne fila er oprinneleg i GML format
og blei konvertert til csv med online verktøyet https://mygeodata.cloud/converter/gml-to-csv
