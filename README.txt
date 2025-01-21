Questo repository contiene un notebook Jupyter (main.ipynb) che contiene tutti i passaggi guidati necessari per riprodurre il 
modello di classificazione descritto nel paper "Towards the identification of essential genes using targeted genome sequencing and comparative analysis".

Dipendenze:
Il codice utilizza le seguenti librerie Python:
- pandas
- numpy
- matplotlib.pyplot
- sklearn 
  - sklearn.model_selection.train_test_split
  - sklearn.naive_bayes.CategoricalNB
  - sklearn.preprocessing.LabelEncoder
  - sklearn.ensemble.RandomForestClassifier
  - sklearn.metrics.roc_auc_score, roc_curve, auc
  - sklearn.model_selection.StratifiedKFold


Requisiti:
Il codice si aspetta di trovare i seguenti dataset nella cartella /assets:
    - cerevisiae_data.xls
    - coli_data.xls
    - paper_results.xls

I file possono essere scaricati dalla sezione "Electronics supplementary material" del paper, disponibile al seguente link: https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-7-265#Sec30. I file corrispondenti sono:
    - Additional file 3: cerevisiae_data.xls
    - Additional file 4: coli_data.xls
    - Additional file 6: paper_results.xls

Nota:
- Nel Additional file 4 (dataset per Escherichia coli), sono presenti problemi di formattazione nei label delle colonne, che variano tra i due fogli del file. Gli spazi nei nomi delle colonne sono stati sostituiti con underscore per garantire una corretta gestione dei dati nel codice.