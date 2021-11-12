The purpose of this analysis is to use a neural network to review and analyze date to help Alphabet Soup determine which companies should receive loans from them.  The TensorFlow library is used to creae, train and evaluate the data.

PROCESS

The data was preprocessed by removing 'EIN' and 'NAME' columns as they added no relevant data.  Further, columns containing categorical data were converted to numerical data and limits were set to cut off outliers.  After this was complete the target was determined to be whether the loan was (therefore predicting will be) successful and the features were all other columns.
MODELING
The data was then put into a test/train framework and using neural networks varous configurations were run in an attempt to get to 75% accuracy

SUMMARY of MODELS

Model 1
I used two layers with 10 and 5 nuerons respectively.  

Outcome:
268/268 - 0s - loss: 0.5686 - accuracy: 0.7264 - 456ms/epoch - 2ms/step
Loss: 0.5686147212982178, Accuracy: 0.7264139652252197

Model 2
I adjusted the neurons to 2 and 7 respectively.  Unsuprising, the outcome was worse.  

Outcome:
268/268 - 0s - loss: 0.5686 - accuracy: 0.7264 - 456ms/epoch - 2ms/step
Loss: 0.5686147212982178, Accuracy: 0.7264139652252197


Model 3
For the third model I added a layer.  The layers have 10, 5 and 3 neurons respectively.

Outcome:
268/268 - 0s - loss: 0.5691 - accuracy: 0.7254 - 419ms/epoch - 2ms/step
Loss: 0.5691158175468445, Accuracy: 0.7253644466400146

Model 4
A final model was developed by using the same layers as Model 3, but also dropping Income Amount.  

Outcome:
268/268 - 0s - loss: 0.5581 - accuracy: 0.7286 - 419ms/epoch - 2ms/step
Loss: 0.5580678582191467, Accuracy: 0.7286297082901001

SUMMARY
I was unable to develop a model in 4 attempts to achieve 75% accuracy
