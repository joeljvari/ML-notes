# ML Notes
This contains full ML notes and the sample codes related to ML

## what is Machine Learning?
Field of study that gives the computer the ability to learn without explicitly programmed.

## Meachine Learning Alogorithms:
- Supervised learning 
- Unsupervised learning
- Reinforcement Learning
- Recommender system

### Supervised Learning:
In supervised machine learning, we are learning to create models that combine inputs, to produce useful predictions even on previously unseen data.
**"Right answer"** is given
- Regression: predict continous valued output
- classification: Discret valued output(1 or 0)

**Support Vector Machine : It has infinite no of features or attribuites**  

![alt text](https://raw.githubusercontent.com/joeljvari/ML-notes/master/breast%20cancer.PNG "fig-1 :Classification Problem Example")

![alt text](https://raw.githubusercontent.com/joeljvari/ML-notes/master/house%20price.PNG "fig-1 :Regression Problem Example")

### Terminology:
- **Label is the varible that we are predicting**
- **Features are the input varibles that are describing our data.**
- **Example is a particular instance of data, x **
     - Labeled example has {features, label}: (x, y)
            Used to train the model
     - Unlabeled example has {features, ?}: (x, ?)
            Used for making predictions on new data
- **Model maps examples to predicted labels: y'**
           defines the relationship between features and label.
     - Training means creating or learning the model. That is, you show the model labeled examples 
           and enable the model to gradually learn the relationships between features and label.
     - Inference means applying the trained model to unlabeled examples. 
           That is, you use the trained model to make useful predictions (y').                 

**Loss:**
A Convenient Loss Function for Regression
L2 Loss for a given example is also called squared error
= Square of the difference between prediction and label
= (observation - prediction)2
= (y - y')2
![alt text](https://raw.githubusercontent.com/joeljvari/ML-notes/master/house%20price%20vs%20sq%20foot.PNG "fig-3")

**Defining L2 Loss on a Data Set:**
 loss function called squared loss (also known as L2 loss)
when we are training our model we care about minimising loss across the entire datasets
![alt text](https://raw.githubusercontent.com/joeljvari/ML-notes/master/Defining%20L2%20Loss%20on%20a%20Data%20Set.PNG "fig-4")

**Mean square error (MSE) is the average squared loss per example over the whole dataset**
![alt text](https://raw.githubusercontent.com/joeljvari/ML-notes/master/MSE.PNG "fig-5")

### **Training :**
 Training a model simply means learning (determining) good values for all the weights and the bias from labeled examples.            
 In supervised learning, a machine learning algorithm builds a model by examining many examples and attempting to find a model that minimizes loss; this process is called **empirical risk minimization.**
 
### Reducing Loss:
To train a model, we need a good way to reduce the model’s loss. 
An iterative approach is one widely used method for reducing loss.
 
