# Stock_Price_Prediction


In order to run the code, you need to create a folder in your google drive named 'kaggle', (without the quotes)
Place 'prices.csv' in there.

Then click runtime->run all.

You need to go to the cell where google drive is mounted and follow the link and enter your authorization code.
Also if you have prices.csv and not a zip file, you go to the cell where prices.csv.zip is unzipped and enter no or yes(for the CNN).

After that it should run the rest of the code and output the results.

CNN’s are specialized types of neural networks that are designed to work with 2-dimensional image data. A CNN consists of two processing layers: the convolutional layers and the pooling layers (Mehtab, 2020). The convolutional layer reads the input in the form of 2-dimensional images and captures the dependencies in an image by using relevant filter mapping. These filter maps reduce the number of parameters without losing any relevant features. The pooling layer uses the feature mapping to capture the relevant image features. By filtering the image data, the pooling layer reduces the dimension of the image data, thus reducing the computational power needed to process the data (Saha, 2018).

In this project, the CNN model (as shown in figure 1) consists of one 2-dimensional convolution layer that extracts 8 feature maps. The input that layer reads is a time series forecasting from the Google stock price dataset that has been converted to a 2-dimensional image vector. The model uses a Max Pooling layer, a type of pooling layer that returns the maximum values of pixels of the image covered by the filter map. This step helps in reducing the dimension of the image data and also removes noise from data. The output image data is then converted into a 1 dimensional vector for the dense layers. The dense layer is a fully connected hidden layer used to learn non-linear combinations of data. A dropout layer is used to regularize data and remove overfitting. The performance of the layers is optimized by using the adam optimizer, a version of the stochastic gradient descent algorithm, with a learning rate of 0.01. We trained the model using 100 epochs and a batch containing 64 input values (Mehtab, 2020). Finally, the accuracy of the model is tested using the root mean square error (RMSE).

Saha, Sumit. “A Comprehensive Guide to Convolutional Neural Networks - the ELI5 Way.” Medium, Towards Data Science, 17 Dec. 2018, towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53. 
Mehtab, Sidra, and Jaydip Sen. “Stock Price Prediction Using CNN and LSTM-Based Deep Learning Models.” 2020 International Conference on Decision Aid Sciences and Application (DASA), 2020, doi:10.1109/dasa51403.2020.9317207.
