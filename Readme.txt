Deep learning neural networks have shown promising results in problems related to vision, speech and 
text with varying degrees of success. I have tried looking at a text problem here, where we are trying 
to predict gender from name of the person. RNNs are a good fit for this as it involves learning from sequences
 (in this case sequence of characters).we will use character sequences which make up the name as our X variable, 
with Y variable as m/f indicating the gender. we use a stacked LSTM model and a final dense layer with softmax 
activation (many-to-one setup). categorical cross-entropy loss is used with adam optimizer. 
A 20% dropout layer is added for regularization to avoid over-fitting.

Step -1 Importing required Libraries

Step -2 Google drive Mount for Importing input data CSV

Step -3 Path is given from Google drive

Step -4 Only alphabets are filtered .Numerics and spacial Characters are removed

Step -5 Identifying Vocabulary and length of vocabulary words

Step -6 Train Test spliting

Step -7 Take input upto max and truncate rest
        Encode to vector space(one hot encoding)
        also convert each index to one-hot encoding

Step -8 Model Building,Fitting and Hyperparameters are tuned to get reasonable test accuracy


