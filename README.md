# Employee-productivity-prediction

## 1. Summary
The goal of this project is to predict the actual productivity of garment employees by using deep learning 

The dataset is obtained from [Employee-productivity](https://www.kaggle.com/datasets/ishadss/productivity-prediction-of-garment-employees).

## 2. IDE and Framework
This project is created using Sypder 5.3.1 as the main IDE. The main frameworks used in this project are Pandas, Numpy, Scikit-learn and TensorFlow Keras.

## 3. Methodology
### 3.1. Data Pipeline
The data is first loaded and preprocessed, such that unwanted features are removed. Categorical features are label encode. Then the data is split into train-validation-test sets, with a ratio of 60:20:20.

### 3.2. Model Pipeline
A feedforward neural network is constructed that is catered for regression problem. The structure of the model is fairly simple. Figure below shows the structure of the model.

![model](https://user-images.githubusercontent.com/108482217/176981780-075c50ef-670d-4579-9bcb-6bedcd609940.png)

The model is trained with a batch size of 128 and for 1000 epochs. Early stopping is applied in this training. The figures below show the graph of the training process, indicating the convergence of model training.

![loss](https://user-images.githubusercontent.com/108482217/176981784-6725cf77-fa59-4506-9cbe-d28093e8e748.png)

## 4. Results
The model are tested with test data. The evaluation result is shown in figure below.

![test_result](https://user-images.githubusercontent.com/108482217/176981791-4aac230d-7c2a-430c-ab03-41820987c82d.png)

The model is also used to made prediction with test data. A graph of prediction vs label is plotted, as shown in the image below.

![result](https://user-images.githubusercontent.com/108482217/176981796-2f578dae-85e3-4659-8cdf-c78e322c88cf.png)

Based on the graph, a clear trendline of y=x can be seen, indicating the predictions are fairly similar as labels. However, several outliers can be seen in the graph.
