# My MNIST Handwritten Digit Classifier
This project demonstrates how to classify handwritten digits from the MNIST dataset using Logistic Regression in Python. 

## How It's Made:

**Tech used:** Python, scikit-learn, NumPy, Matplotlib, Jupyter Notebook

Here are some of the steps I took when building:
1. Data Loading: Pulled the MNIST dataset (mnist_784) from OpenML with fetch_openml.
2. Visualization: Displayed sample digits by reshaping the pixel vectors into 28×28 images.
3. Model Training: Split the dataset into training and test sets, then trained a Logistic Regression classifier.
4. Evaluation: Measured accuracy on the test set and built a confusion matrix to analyze misclassifications.
5. Visualization of Results: Plotted a heatmap confusion matrix with annotated counts for each digit.
This project highlights both the usefulness of simple linear models for image recognition tasks and the importance of visualization for understanding model behavior.

## Lessons Learned:

The Logistic Regression model achieved strong overall accuracy on the MNIST dataset, performing particularly well on digits with more distinctive shapes such as 0, 1, and 9. 
These digits were classified correctly at very high rates, as shown in the confusion matrix, because their pixel patterns are relatively easy for the model to distinguish. 

However, the model also showed some weaknesses, especially with digits that share similar structures. For example, the confusion matrix revealed misclassifications between 3 and 5, as well as 4 and 9, 
which often share overlapping stroke patterns in handwritten form. These results highlight both the strength of the model in recognizing clear, unambiguous digit shapes and its limitations in handling
digits that are visually more confusable.

## Links to resources:

mnist_784 dataset: https://www.openml.org/search?type=data&status=active&id=554
LBFGS algorithm: https://en.wikipedia.org/wiki/Limited-memory_BFGS

