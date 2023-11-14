# Classification_of_images
### train_test_data
https://drive.google.com/drive/folders/1iCi3XvoFl1-64U39LUGTTIi7COAsGkBw?usp=sharing
### project_notebook.ipynb
This is a classification issue.
We have flower photo data in 5 categories and we want to train a model to estimate the category of that photo (which is one of these 5 categories) by taking a photo.
At first, we import the training data into RAM in batches.
Then using the pre-trained EfficientNetB6 model
We train a model that has these specifications:
Total parameters: 42,195,598
Trainable parameters: 1,235,455
losses: SparseCategoricalCrossentropy
optimizer: Adam(learning_rate=0.0001)
class_weight: {0: 1.42, 1: 1., 2: 1.38, 3:1.49, 4:1.07}
Then we compiled our own model and fitted it to the data.
whose loss diagram is as follows:
p
And after that, we read the test data one by one and identified their categories, then we created a csv file of the names of the photos and their categories.
### sample_submission.csv
