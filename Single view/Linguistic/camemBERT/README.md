# Description

This repository includes the clustering (conventional and HistStream) results of dataset **_camemBERT_pause_LSTM.pickle_**

## First step -- Select the final representative dataset for clustering application.

- **_camemBERT_pause_LSTM_** : dataset obtained by applying $${\color{#326a95}camamBERT+LSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_camemBERT_pause_BiLSTM_** : dataset obtained by applying $${\color{#326a95}camamBERT+BiLSTM}$$ as burst embedding model, trained to predict pause duration ($${\color{#326a95}pause}$$);
- **_camemBERT_pctpause_LSTM_** : dataset obtained by applying $${\color{#326a95}camamBERT+LSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctause}$$);
- **_camemBERT_pctpause_BiLSTM_** : dataset obtained by applying $${\color{#326a95}camamBERT+BiLSTM}$$ as burst embedding model, trained to predict percentage of the pause duration ($${\color{#326a95}pctpause}$$);

<p align="center">
  <img src="./ClusRes_images/conv_res.png" alt="conv_res.png">
  <br>
  <b> Fig1. Mean results of all clustering algorithms (using convnetional approaches)</b>
</p>

<p align="center">
  <img src="./ClusRes_images/hist_res.png" alt="conv_res.png">
  <br>
  <b>Fig2. Mean results of all clustering algorithms (using proposed HistStream framework) </b>
</p>

According to the mean results of each representation (tables above), choose the one that wins the most times in the 'Best candidate':

- pause_simpleLSTM (7 times)
- pctpause_doubleLSTM (1 time)

Finally, $${\color{#f48522}pause_simpleLSTM}$$ is chosen as the final representation based on CamemBERT with saved file name : _camemBERT_pause_LSTM.pickle_



