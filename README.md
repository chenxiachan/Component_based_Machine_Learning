# Component_based_Machine_Learning
Open source code of paper: <br>
*Utilizing Domain Knowledge: Robust Machine Learning for Building Energy Prediction with Small, Inconsistent Datasets*<br>
Paper: 
[[Arxiv]](https://arxiv.org/abs/2302.10784)

In this paper, we use inductive logic and disentanglement to separate the compositionality of the building semantic information. By embedding such information into the ML organization with trained ML models for building components and zones, the Component-based machine learning (CBML) framework successfully predicts new building designs’ performance with the following advantages. 
1. Robustness against sparse, noisy data inputs.
2. Efficient data utilization from different entities.
3. Accepting incomplete data with high interpretability and reduced training time.
4. Reducing difficulties/costs in real-world industry deployment. 


---
![image](https://github.com/chenxiachan/Component_based_Machine_Learning/assets/106488602/a928192f-ba2d-47fe-88c6-8a1c6ae1f7f9)
*Two predictive modeling strategies and the dataset (a) the dataset generated for training/test sets in different building shapes. In this study, we use a box-shape buildings dataset for model training using (b) monolithic ML model and (c) component-based ML model strategies. Both approaches are then validated on test datasets in box-shape, random shapes, and representative buildings.*


---
For running the code, please first download the data from:
[[Mendeley Data]](https://data.mendeley.com/datasets/fctghwx3r9/2)

Run notebook `0_Data_Preprocessing.ipynb`, `1_Monolithic_Forecasting.ipynb`, and `2_CBML_Forecasting.ipynb` in sequential. <be>

The following additional python packages are required:
`pip install pandas numpy matplotlib seaborn lightgbm scikit-learn tqdm plotly`

For using the code or data, please cite:<br>

- *Chen, X., Singh, M.M. and Geyer, P., 2023. Utilizing Domain Knowledge: Robust Machine Learning for Building Energy Prediction with Small, Inconsistent Datasets. arXiv preprint arXiv:2302.10784.*
- *CHEN, Xia; Singh, Manav Mahan; Geyer, Philipp (2023), “Utilizing domain knowledge: robust machine learning for building energy performance prediction with small, inconsistent datasets”, Mendeley Data, V2, doi: 10.17632/fctghwx3r9.2*


---
![image](https://github.com/chenxiachan/Component_based_Machine_Learning/assets/106488602/e0d7a107-2eee-4897-a064-aeb4a8990f70)
*Generalization via prior knowledge encoding: (a) The scope of problem space: The knowledge-encoded ML (CBML) allows data collection from different building instances (certain types of building design space), trains ML component models through building semantic abstraction, and predict new buildings by reassembling components; It transfers the ML prediction problem from extrapolation to interpolation and cover a larger problem space; (b) Monolithic modeling: extrapolation problem; (c) Component-based machine learning: interpolation problem; It overcomes the limitation of requiring complete input collection from buildings and maximizes the data utility.*

---
![image](https://github.com/chenxiachan/Component_based_Machine_Learning/assets/106488602/d9b552f8-44fa-4f8d-8ddc-dd089d841df7)
*Accuracy result comparison on different test datasets. LightGBM models are trained on different sparseness of the training data (sampling rate) from 1.00% to 0.0125%.*
