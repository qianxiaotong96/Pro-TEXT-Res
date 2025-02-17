# Description

This repository includes the clustering (conventional and HistStream) results of dataset **_camemBERT_pause_LSTM.xlsx_**

## First step -- select final dataset to apply clustering

- **_camemBERT_pause_LSTM.xlsx_** : dataset obtained by applying $${\color{#326a95}camamBERT+LSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_camemBERT_pause_BiLSTM.xlsx_** : dataset obtained by applying $${\color{#326a95}camamBERT+BiLSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_camemBERT_pctpause_LSTM.xlsx_** : dataset obtained by applying $${\color{#326a95}camamBERT+LSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctause}$$);
- **_camemBERT_pctpause_BiLSTM.xlsx_** : dataset obtained by applying $${\color{#326a95}camamBERT+BiLSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctpause}$$);

<p align="center">
  <img src="./ClusRes_images/conv_res.png" alt="conv_res.png">
  <br>
  <span style="font-family: italic> "Fig1. Mean results of all clustering algorithms (using convnetional approaches)</span>
</p>

<p align="center">
  <img src="./ClusRes_images/hist_res.png" alt="conv_res.png">
  <br>
  <b>Fig2. Mean results of all clustering algorithms (using proposed HistStream framework) </b>
</p>


