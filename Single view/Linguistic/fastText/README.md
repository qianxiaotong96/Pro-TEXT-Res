# Description

This repository includes the clustering (conventional and HistStream) results of dataset **_fastText_pause_LSTM.pickle_**

## First step -- Select the final representative dataset for clustering application.

- **_fastText_pause_LSTM_** : dataset obtained by applying $${\color{#326a95}fastText+LSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_fastText_pause_BiLSTM_** : dataset obtained by applying $${\color{#326a95}fastText+BiLSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_fastText_pctpause_LSTM_** : dataset obtained by applying $${\color{#326a95}fastText+LSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctause}$$);
- **_fastText_pctpause_BiLSTM_** : dataset obtained by applying $${\color{#326a95}fastText+BiLSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctpause}$$);

<p align="center">
  <img src="./ClusRes_images/conv_res.png" alt="conv_res.png">
  <br>
  <b>Fig1. Mean results of all clustering algorithms (using convnetional approaches)</b>
</p>

<p align="center">
  <img src="./ClusRes_images/hist_res.png" alt="hist_res.png">
  <br>
  <b>Fig2. Mean results of all clustering algorithms (using proposed HistStream framework)</b>
</p>

According to the mean results of each representation (tables above), choose the one that wins the most times in the 'Best candidate':

- pause_simpleLSTM (5 times)
- pause_doubleLSTM (2 times)
- pctpause_simpleLSTM (1 time)

Finally, **pause_simpleLSTM** is chosen as the final representation based on fastText with saved file name : **_fastText_pause_LSTM.pickle_**

```python
# Load dataset 

>>> import pickle
>>> with open('fastText_pause_LSTM.pickle', 'rb') as f:
      x = pickle.load(f)
>>> x.shape
... (5051, 150)
```
## Second step -- Clustering application

<p align="center">
  <img src="./ClusRes_images/conv_visualization.png" alt="conv_visualization.png">
  <br>
  <b>Fig3. Clustering visualization of each clustering algorithm (using convnetional approaches)</b>
</p>

<p align="center">
  <img src="./ClusRes_images/conv_mean_Summary.png" alt="conv_mean_Summary.png">
  <br>
  <b>Fig4. Mean results of each clustering algorithm (using convnetional approaches)</b>
</p>

**Agglomerative** win the most, save the clustering results in the file named **_fastText_pause_LSTM_Agglomerative.xlsx_** 

<p align="center">
  <img src="./ClusRes_images/hist_visualization.png" alt="hist_visualization.png">
  <br>
  <b>Fig5. Clustering visualization of each clustering algorithm (using proposed HistStream framework)</b>
</p>

<p align="center">
  <img src="./ClusRes_images/hist_mean_Summary.png" alt="hist_mean_Summary.png">
  <br>
  <b>Fig6. Mean results of each clustering algorithm (using proposed HistStream framework)</b>
</p>

**DBSCAN_HistStream** win the most, save the clustering results in the file named **_fastText_pause_LSTM_DBSCAN_HistStream.xlsx_** 

## Summary

- Burst embedding results for use : **_fastText_pause_LSTM.pickle_**   
- Clustering results : **_fastText_pause_LSTM_Agglomerative.xlsx_** and **_fastText_pause_LSTM_DBSCAN_HistStream.xlsx_**

($\color{red}{\text{The clustering result files contain the original dataset information and a new column called 'label/class' which indicates the clustering results.}}$)
