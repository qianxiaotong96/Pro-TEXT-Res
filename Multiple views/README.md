# Summary
After the steps of selecting the representative dataset in Single view section, the composition of multi-view datastes could be summarized as follow :

| MvDataset Name        | Semantic view                           | Static view   | Linguistic view        |
| --------------------- | --------------------------------------- | ------------- | ---------------------- |
| **_mvProTEXT_0_**     | _sentenceTransformer_pctpause_          |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_1_**     | _sentenceTransformer_pctpause_          |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_2_**     | _sentenceTransformer_pctpause_          |  _statistic_  | _word2vec_pause_LSTM_  | 
| **_mvProTEXT_3_**     | _sentenceTransformerCamemBERT_pctpause_ |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_4_**     | _sentenceTransformerCamemBERT_pctpause_ |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_5_**     | _sentenceTransformerCamemBERT_pctpause_ |  _statistic_  | _word2vec_pause_LSTM_  | 
| **_mvProTEXT_6_**     | _camemBERT_pause_LSTM_                  |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_7_**     | _camemBERT_pause_LSTM_                  |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_8_**     | _camemBERT_pause_LSTM_                  |  _statistic_  | _word2vec_pause_LSTM_  | 
| **_mvProTEXT_9_**     | _SpaCy_pause_LSTM_                      |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_10_**    | _SpaCy_pause_LSTM_                      |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_11_**    | _SpaCy_pause_LSTM_                      |  _statistic_  | _word2vec_pause_LSTM_  | 
| **_mvProTEXT_12_**    | _fastText_pause_LSTM_                   |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_13_**    | _fastText_pause_LSTM_                   |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_14_**    | _fastText_pause_LSTM_                   |  _statistic_  | _word2vec_pause_LSTM_  | 
| **_mvProTEXT_15_**    | _word2vec_pause_LSTM_                   |  _statistic_  | _camemBERT_pause_LSTM_ |
| **_mvProTEXT_16_**    | _word2vec_pause_LSTM_                   |  _statistic_  | _fastText_pause_LSTM_  |
| **_mvProTEXT_17_**    | _word2vec_pause_LSTM_                   |  _statistic_  | _word2vec_pause_LSTM_  | 

And we could find in the following figures a simple visualization of each dataset with t_SNE dimension reduction 

