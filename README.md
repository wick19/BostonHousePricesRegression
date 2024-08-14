# Using MULTI-LAYER PERCEPTION for The Boston House Prices Regression Dataset by using PyTorch :

**Synopsis:**

**Problem Statement:**
* Aimed to build a price prediction model using an MLP network considering 13 variables such as CRIM, Age, etc.

**Data Loading and Preprocessing:**
* Loaded the Boston housing dataset using sklearn's load_boston() function and converted it into a pandas DataFrame for easier manipulation.
* To ensure uniformity across variables, I standardized the features using StandardScaler.

**Data Visualization:**
* Created a scatter plot of the average number of rooms (RM) against prices (PRICES) to visualize their relationship.

**Model Building:**
* For constructing the MLP model, PyTorch was used PyTorch. The model consists of an initial linear layer accommodating the 13 input variables, ReLU activation functions for non-linearity, and a linear output layer.
* To review the model's architecture, it printed its layers and configurations.
  
**Training the Model:**
* Converting the data into tensors, optimized the model using Mean Squared Error (MSE) as the loss function and the Adam optimizer.
* The model underwent training for 200 epochs, with periodic printing of the loss to monitor progress.

**Model Evaluation:**
* After training, I made predictions on both training and testing sets.
* To assess the model's performance on the testing set, calculated the R-squared (R2) score.

**Results Visualization:**
* Visualized the predicted prices against the actual prices for both training and testing sets using a scatter plot.
* The plot illustrated how well the model's predictions aligned with the actual values, with red and blue circles denoting training and testing data, respectively.

# Training Process Explanation:
At each epoch, the model went through a series of steps: initializing the gradient of the model parameters, calculating the loss, backpropagating to compute the gradient of the model parameters, and updating the model parameters.
With the number of epochs set to 200, these steps were repeated to gradually decrease the loss, indicating progress in training.

# Summary: 
Project showcases my approach to building and training an MLP model for price prediction using the Boston housing dataset. Leveraging libraries such as sklearn, pandas, NumPy, Matplotlib, seaborn, and PyTorch, I demonstrated a comprehensive methodology for machine learning model development.
