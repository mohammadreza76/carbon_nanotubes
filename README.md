# carbon_nanotubes
machine learning-regression-svr-scikit-learn

# About Dataset(information from https://www.kaggle.com/inancigdem/carbon-nanotubes):
This dataset contains 10721 initial and calculated atomic coordinates of carbon nanotubes (CNTs) and their chiral networks obtained from a simulation software named as BIOVIA Materials Studio CASTEP (CASTEP).
CASTEP can simulate a wide range of properties of materials proprieties using density functional theory (DFT). DFT is the most successful method calculates atomic coordinates faster than other mathematical approaches, and it also reaches more accurate results. The dataset is generated with CASTEP using CNT geometry optimization. Many CNTs are simulated in CASTEP, then geometry optimizations are calculated. Initial coordinates of all carbon atoms are generated randomly. Different chiral vectors are used for each CNT simulation. The atom type is selected as carbon, bond length is used as 1.42 A° (default value). CNT calculation parameters are used as default parameters. To finalize the computation, CASTEP uses a parameter named as elecenergytol (electrical energy tolerance) (default 1x10-5 eV) which represents that the change in the total energy from one iteration to the next remains below some tolerance value per atom for a few self-consistent field steps. Initial atomic coordinates (u, v, w), chiral vector (n, m) and calculated atomic coordinates (u’, v’, w’) are obtained from the output files.
The summary of the attributes is given below. Please read the papers (https://doi.org/10.1007/s00339-016-0153-1 and https://doi.org/10.17341/gazimmfd.337642) for detailed descriptions of the attributes. 

Chiral indice n: n parameter of the selected chiral vector.
Chiral indice m: m parameter of the selected chiral vector.
Initial atomic coordinate u: Randomly generated u parameter of the initial atomic coordinates of all carbon atoms.
Initial atomic coordinate v: Randomly generated v parameter of the initial atomic coordinates of all carbon atoms.
Initial atomic coordinate w: Randomly generated w parameter of the initial atomic coordinates of all carbon atoms.
Calculated atomic coordinate u’: Calculated u’ parameter of the atomic coordinates of all carbon atoms.
Calculated atomic coordinate v’: Calculated v’ parameter of the atomic coordinates of all carbon atoms.
Calculated atomic coordinate w’: Calculated w’ parameter of the atomic coordinates of all carbon atoms.

# About Project:
I used Linear Regression and Svr model(with k-fold cross validation) for predicting Calculated atomic coordinates(u',v',w') for carbon_nanotubes dataset with scikit-learn.
in this dataset we have 5 features and more than 10000 samples.

In Linear Regression model i got 99% accuracy and in Svr model(with k-fold cross validation) i got 95.9% accuracy in avrage.
In this project i used sckit-learn,pandas,matplollib libraries.
