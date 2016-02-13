# In-Class Kaggle Competitions

## Harvard CS181 Machine Learning - Spring 2016

**[Competition 1](https://inclass.kaggle.com/c/cs181-s16-practical-1-predicting-the-efficiency-of-photovoltaic-molecules):** Predicting the Efficiency of Organic Photovoltaic Molecules

What if you could capture and convert sunlight into electricity with a material as cheap and as versatile as a plastic bag? What if the material could be produced on a massive scale, with easily accessible technology? What if other versions of the material could be coated, painted, or sprayed on building surfaces for solar energy production? What if these materials were ultra-thin and ultra-light for portable devices? And finally, what if they were inexpensive and could provide electricity to people in the developing world?  — Harvard Clean Energy Project

Solar power is one of the most promising technologies for renewable energy to reduce our dependence on fossil fuels. Unfortunately, most modern solar cells are based on silicon. These materials are rigid, expensive, and difficult to manufacture. On the other hand, \emph{carbon} based solar cells could be cheap to produce, flexible, transparent, and be made and molded as easily as plastics. There's just one catch: no known organic photovoltaic molecules are as efficient as their silicon counterparts.

The Harvard Clean Energy Project has been using massive scales of computation to explore new possibilities for organic photovoltaics. The project uses density functional theory (DFT) to estimate the the properties of the molecules that determine their potential efficiency as solar cells. The main quantity of interest is the difference in energy between the highest occupied molecular orbital (HOMO) and the lowest unoccupied molecular orbital (LUMO). It can take hours or days to compute this accurately on a modern computer.

Recently, it has become clear that machine learning might have something to say about this. It may be possible to sidestep these expensive DFT computations by learning a function from a feature representation of the molecule to the HOMO-LUMO gap. From our point of view in CS181, this is a regression problem: take molecular features and produce a real-valued prediction of what the DFT would calculate. Better machine learning models for this problem could lead to new kind of materials and more efficient solar cells!

You have one million molecules to train on, and are tasked with making predictions on another 800,000 or so. You'll upload your predictions to Kaggle, where a subset will be used to produce a ``public leaderboard'' and another subset will be used to reveal the final rankings at the end of the contest. You'll have access to complete information about the molecular structure in the form of a SMILES string. This is a representation that chemists like to use to encode molecular structures. Here is an example:

c1sc(-c2sc(-c3ccc(cc3)-c3scc4sccc34)c3[se]ccc23)c2sccc12

One of the challenges of making predictions about molecules is finding a good feature representation. Clearly, the SMILES string itself isn't going to be all that helpful. Luckily, many chemists have built tools to build interesting representations. One such tool is a Python package called RDKit. With it you can easily load SMILES strings and produce features. Alternatively, you can just use the features we've already extracted with RDKit, which produced 256-dimensional binary vectors. These vectors are in the training and test files provided.




**Team Members:**

Gioia Dominedo  |  [@dominedo](https://github.com/dominedo)  |  dominedo@g.harvard.edu

Amy Lee  |  [@amlsf](https://github.com/amlsf)  |  amymaelee@g.harvard.edu

Kendrick Lo  |  [@ppgmg](https://github.com/ppgmg)  |  klo@g.harvard.edu
