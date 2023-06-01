# Machine Learning Trading Evaluation Report

## What impact resulted from increasing or decreasing the training window?

To adjust the size of the training dataset, you can use a different DateOffset value—for example, six months. Be aware that changing the size of the training dataset also affects the size of the testing dataset.

1. baseline performance:
Using the VSC model, with a short window of 4 and a long window of 100, the data will be sliced for training for a period of 3 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-07-02 15:00:00. The data for testing will be from 2015-07-06 10:00:00 to 2021-01-22 15:45:00.
![figure1.png](Resources/figure1.png)

2. Increasing the training window
Using the VSC model, with a short window of 4 and a long window of 100, the data will be sliced for training for a period of 6 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-10-02 15:00:00. The data for testing will be from 2015-10-06 10:00:00 to 2021-01-22 15:45:00.
![figure2.png](Resources/figure2.png)

---------------------------------------------------------------------------

## What impact resulted from increasing or decreasing either or both of the SMA windows?
Using the VSC model, with a short window of 4 and a long window of 150, the data will be sliced for training for a period of 6 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-10-02 15:00:00. The data for testing will be from 2015-10-06 10:00:00 to 2021-01-22 15:45:00.
![figure3.png](Resources/figure3.png)

Using the VSC model, with a short window of 5 and a long window of 160, the data will be sliced for training for a period of 6 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-10-02 15:00:00. The data for testing will be from 2015-10-06 10:00:00 to 2021-01-22 15:45:00.
![figure4.png](Resources/figure4.png)

---------------------------------------------------------------------------

## Choose the set of parameters that best improved the trading algorithm returns. 

Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

1. Use LogisticRegression model
Using the LogisticRegression model, with a short window of 4 and a long window of 100, the data will be sliced for training for a period of 3 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-07-02 15:00:00. The data for testing will be from 2015-07-06 10:00:00 to 2021-01-22 15:45:00.
![figure1.png](Resources/figure5.png)

2. Use DecisionTree modelß
Using the DecisionTree model, with a short window of 4 and a long window of 100, the data will be sliced for training for a period of 3 months. The training data will begin at 2015-04-02 15:00:00 and end at 2015-07-02 15:00:00. The data for testing will be from 2015-07-06 10:00:00 to 2021-01-22 15:45:00.
![figure1.png](Resources/figure6.png)

3. Use Nerual Network

Using Nerual Network model with 3 hidden nodes layers.create data features as EMA_D3,EMA_D5,EMA_D8,EMA_D10,EMA_D12,EMA_D15,EMA_D30,EMA_D35,EMA_D40,EMA_D45,EMA_D50,EMA_D60, and data labels are signals 1, -1.the data are sliced for training for a period of 12 months. 