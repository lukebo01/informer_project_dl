# Informer-Based Long Series Forecasting

## Descrizione del Progetto
Questo progetto implementa il modello **Informer** per il **long series forecasting**, con dataset caratterizzati da **alta stagionalità** e **non linearità**. L'obiettivo è confrontare l'Informer con modelli standard come LSTM, ARIMA ecc.. e valutarne le prestazioni su uno o più dataset.

## Requisiti di Sistema
- **Python 3.7** (obbligatorio, a causa di compatibilità con Informer2020)
- **Sistema operativo**: Linux/macOS/Windows
- **CUDA (opzionale)**: per l'accelerazione su GPU

## Installazione

### 1. Clonare il Repository
```sh
# Clona il progetto
git clone https://github.com/lukebo01/informer_project_dl.git
cd informer_project_dl
```

### 2. Creare un Virtual Environment
Si consiglia di usare un ambiente virtuale per gestire le dipendenze.
```sh
# Creazione di un virtual environment
python3.7 -m venv .venv

# Attivazione dell'ambiente virtuale
# Su macOS/Linux:
source .venv/bin/activate
# Su Windows:
.venv\Scripts\activate
```

### 3. Installare le Dipendenze
Le librerie utilizzano versioni specifiche compatibili con **Informer2020**.
```sh
pip install -r requirements.txt
```

> ⚠️ **Nota:** Se vuoi eseguire il modello su GPU, assicurati di installare la versione corretta di **PyTorch** per la tua versione di CUDA.



## Struttura del Progetto
```bash
informer_project_dl/
│── .venv/
│── data/
│   ├── final/
│   ├── raw/
│── informer_checkpoints/
│   ├── informer_custom_fTM_sI96_lI48_pI96_dm512_nh8_el3_dl2_df2048/
│   ├── informer_ETTh1_fTM_sI96_lI48_pI24_dm512_nh8_el2_dl1_df2048/
│── Informer2020/
│   ├── data/
│   ├── exp/
│   ├── models/
│   ├── scripts/
│   ├── utils/
│   ├── main_informer.py
│   ├── requirements.txt
│── experiment_predictive_maintenance.ipynb
│── etth_train_test.ipynb
│── validateDataset.ipynb
│── README.md
│── requirements.txt
│── .gitignore

```

## Link ai Dataset
Di seguito i link per scaricare i dataset adatti all' informer:

- **ETT Dataset (Electricity Transformer Temperature)**: [ETT Download](https://github.com/zhouhaoyi/ETDataset)
- **M4 Dataset (Finance, Industry, Macro, Demography)**: [M4 Download](https://www.kaggle.com/competitions/m4-forecasting)
- **PeMS Traffic Dataset (Flusso di traffico stradale)**: [PeMS Download](https://doi.org/10.5281/zenodo.12247)
- **BDG2 (Building Data Genome 2 - Energia Edifici)**: [BDG2 Download](https://github.com/buds-lab/building-data-genome-project-2)

## Contatti
Per qualsiasi domanda o suggerimento, puoi contattarmi via email: **luc.borreli1@stud.uniroma3.it** oppure aprire una **issue** su GitHub.

---
© 2024, Luca Borrelli. Progetto open-source sotto licenza MIT.
