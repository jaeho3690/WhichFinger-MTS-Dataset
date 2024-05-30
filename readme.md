# WhichFinger Dataset from CAFO: Feature-Centric Explanation on Time Series Classification [![Generic badge](https://img.shields.io/badge/code-official-green.svg)](https://shields.io/)
![Overview](./figures/WhichFinger.png)


This is the WhichFinger Multivariate Time Series (MTS) dataset from the SIGKDD 2024 paper `CAFO: Feature-Centric Explanation on Time Series Classification` by **Jaeho Kim**, Seok-Ju (Adam) Hahn, Yoontae Hwang, Junghye Lee, and Seulki Lee. 
We provide both the raw data, and the preprocessed data. This dataset was designed for explainable AI (XAI) purpose, especially to highlight class-wise importance of features. 


## GoogleDrive Link
https://drive.google.com/drive/folders/16Xks-9O6BeTFHOba9-HZRZcnd2GnrUVg?usp=sharing


## GoogleDrive Contents
- `WhichFinger/raw_data_df.pkl`: This contains the whole raw data. You can load this file in the `notebook/preprocess.ipynb` for preprocessing, or you can use the below.
- `WhichFinger/WhichFinger_ModelTraining`: Containing the preprocessed files used for model training.
- `answer_sheet.csv`: The Answer Sheet used to evaluate the `CWRI` metrics.
- `finger_dataset.py`: A PyTorch Dataset class
- `fingergesture.pkl`: We used this file for model training. It is basically the same file.
- `label_df.csv`: Contains meta info, and `y_true`. 


## Contents
- `notebook/01_preprocess_raw.ipynb`: This notebook contains the preprocessing script for WhichFinger
- `notebook/02_evaluate_cwri.ipynb`: This notebook contains the minimal code to evaluate our CWRI score. 

## Ground Truth Evaluation
![GT](./figures/whichfinger_gt.png)
Please kindly refer to `Appendix E: Evaluation of CWRI Metrics` for further explanation.