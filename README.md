# CS547 (Deep Learning) Project - Group 18 (Beveridge)

# Topic - Port Profiles (#16)

Team members:\
Bryant Zhou (tianyiz8)\
Niket Parikh (niketnp2)\
Sahil Agrawal (sahila4)\
Sai Chetan (scc8)

## Problem Statement

Imports and exports of agricultural goods by the country via sea is one of the main ways that the US earns profits on goods produced and aquires some of its products. It is necessary to know what the expected imports and exports will be in future years, so that we can plan accordingly. This will enable us to judge if our infrastructure is enough to handle these shipments and what the appropriate prices will be. Also, it will enable us to judge how much of a certain product to produce based on the expected import or export; we don't want to be in dearth of a product for which the import will be less.\
So, given past years data on imports and exports of the country measured in metric tons, we want to predict the future export and import in metric tons. Additional information like the port of entry/exit, the type of the product and whether it needs to be refridgerated or not, will allow the prediction for each of these categories individually also (as opposed to the entire import or export). Additionally, to adjust for inflation, we will use the Food CPI inflation of the country to estimate inflation in exports and imports.

## Some Details

### project16.ipynb
The deep neural net is implemented on PyTorch. The baseline method used for comparison to DNN is linear regression, implemented using sklearn. The code is written on Google Colab and the user simply needs to run all the cells in order to obtain the results; epoch average loss (loss function used is mean-squared error (MSE)) during training and MSE on testing set are printed by the program. The data sets used are the pickled files pulled from the project's Google Drive folder.

### Data Statistics.ipynb
This notebook obtains relevant facts about the data such as the number of distinct ports and a high-level idea of skewness of data in terms of data points per month and monthly data points per port.

### train.pkl
The USDA data set has been divided into a training set and validation set. This is the training set. Number of data points in train.pkl is 95% of that in the original data set. The training data points are sampled randomly, using pandas.DataFrame.sample(). The data frame is pickled before saving for computational efficiency.

### debug.pkl
This is the validation data set, consisting of the data points in the original data set but not in train.pkl. The data frame is pickled before saving for computational efficiency.


## License

We currently do not have a fixed license yet. But if we need a license in the future, we will use one of the standard ones like MIT license.
