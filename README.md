# In-Class Kaggle Competitions

## Harvard CS181 Machine Learning - Spring 2016

**[Competition 1](https://inclass.kaggle.com/c/cs181-s16-practical-1-predicting-the-efficiency-of-photovoltaic-molecules):** **Predicting the Efficiency of Photovoltaic Molecules**

For this project we used machine learning methods to predict the potential efficiency of different molecules as building blocks for solar cells, based on molecular structure features encoded in the form of SMILES strings.  More specifically, we produced continuous real-valued predictions of the "gap" that would otherwise be estimated using density functional theory (DFT), where the gap represents the difference in energy between the highest occupied molecular orbital (HOMO) and the lowest unoccupied molecular orbital (LUMO).

At the time of submission, we had uploaded 23 different sets of predictions to Kaggle and achieved a best root mean squared error (RMSE) of 0.053 on the public test data, corresponding to a ranking of 3/86 on the leaderboard. Following release of the withheld final test data (two days later), we achieved a RMSE of 0.054 and a ranking of 5/91 on the leaderboard. Our best results were achieved using a tuned random forest model that used a combination of features, including features from the original dataset, RDKit-generated features associated with molecular bond counts, and counts of contiguous character sequences within the SMILES strings.



**Team Members:**

Gioia Dominedo  |  [@dominedo](https://github.com/dominedo)  |  dominedo@g.harvard.edu

Amy Lee  |  [@amlsf](https://github.com/amlsf)  |  amymaelee@g.harvard.edu

Kendrick Lo  |  [@ppgmg](https://github.com/ppgmg)  |  klo@g.harvard.edu