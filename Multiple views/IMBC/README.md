# Description

This repository includes the best multi-view clustering results of all the MvDatasets 

## First step -- Select the best clustering results by each index.

<p align="center">
  <img src="./ClusRes_images/incr_mv_res.png" alt="conv_res.png">
  <br>
  <b>Fig1. The best 3 clustering results of each evaluation metric in different cases</b>
</p>

According to the results in the table above we choose to save 3 clustering results regarding to each clustering evaluation metric.

- Best mean_CHI : **CMVC** on **_MvProTEXT_14_** dataset with **15** clusters found
- Best mean_SI : **CMVC** on **_MvProTEXT_15_** dataset with **5** clusters found
- Best mean_DBI : **IMBCKMeans** on **_MvProTEXT_14_** dataset with **5** clusters found
  
## Second step -- Clustering visualization

<p align="center">
  <img src="./ClusRes_images/CMVC15_mvProTEXT_14_visualization.png" alt="CMVC15_mvProTEXT_14_visualization.png">
  <br>
  <b>Fig2. t_SNE visualization of CMVC clustering results on "MvProTEXT_14" with 15 clusters founded and best mean_CHI score</b>
</p>

<p align="center">
  <img src="./ClusRes_images/CMVC5_mvProTEXT_15_visualization.png" alt="CMVC5_mvProTEXT_15_visualization.png">
  <br>
  <b>Fig3. t_SNE visualization of CMVC clustering results on "MvProTEXT_15" with 5 clusters founded and best mean_SI score</b>
</p>

<p align="center">
  <img src="./ClusRes_images/IMBCKMeans5_mvProTEXT_14_visualization.png" alt="IMBCKMeans5_mvProTEXT_14_visualization.png">
  <br>
  <b>Fig4. t_SNE visualization of IMBCKMeans clustering results on "MvProTEXT_14" with 5 clusters founded and best mean_DBI score</b>
</p>


The best clustering results are saved in the file named 

- **_CMVC15_mvProTEXT_14.xlsx_**
- **_CMVC5_mvProTEXT_15.xlsx_**
- **_IMBCKMeans5_mvProTEXT_14.xlsx_**

($\color{red}{\text{The clustering result files contain the original dataset information and a new column called 'label/class' which indicates the clustering results.}}$) 
