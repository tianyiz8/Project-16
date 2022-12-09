# CS547 (Deep Learning) Project - Group 18 (Beveridge)

# Topic - Port Profiles (#16)

Team members:\
Bryant Zhou (tianyiz8)\
Niket Parikh (niketnp2)\
Sahil Agrawal (sahila4)\
Sai Chetan (scc8)\

## Problem Statement

Imports and exports of agricultural goods by the country via sea is one of the main ways that the US earns profits on goods produced and aquires some of its products. It is necessary to know what the expected imports and exports will be in future years, so that we can plan accordingly. This will enable us to judge if our infrastructure is enough to handle these shipments and what the appropriate prices will be. Also, it will enable us to judge how much of a certain product to produce based on the expected import or export; we don't want to be in dearth of a product for which the import will be less.\
So, given past years data on imports and exports of the country measured in metric tons, we want to predict the future export and import in metric tons. Additional information like the port of entry/exit, the type of the product and whether it needs to be refridgerated or not, will allow the prediction for each of these categories individually also (as opposed to the entire import or export). Additionally, to adjust for inflation, we will use the Food CPI inflation of the country to estimate inflation in exports and imports.

## Some Details
The deep neural net is implemented on PyTorch. The baseline method used for comparison to DNN is linear regression, implemented using sklearn. The code is written on Google Colab and the user simply needs to run all the cells in order to obtain the results; Epoch average loss (loss function used is mean-squared error (MSE)) during training and MSE on testing set are printed by the program. 


## License

We currently do not have a fixed license yet. But if we need a license in the future, we will use one of the standard ones like MIT license.
