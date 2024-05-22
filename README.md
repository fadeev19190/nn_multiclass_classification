# nn_multiclass_classification

# Using Neural Networks

  * For this assignment, you must construct an appropriate neural network model for multiclass classification.
  * Points will be awarded for both the correctness of your implementation and the final accuracy of your model on the evaluation data.
    
> **Tasks are designed to allow room for creativity. Figuring out _exactly how_ you will solve the assignment is an important part of the task, and originality or ingenuity will also be assessed!**

Use `Markdown` cells to explain your process. Points will be deducted for lack of clarity.

## Data Source

 * The data source consists of `train.csv` and `evaluate.csv` files.
 * These are 32x32 pixel grayscale images derived in some way from the [Fashion MNIST dataset](https://www.kaggle.com/datasets/zalando-research/fashionmnist).
 * The `train.csv` file contains the training data.
 * The target (dependent) variable is named **label**.
 * The `evaluate.csv` file contains the test data without actual label values.

## Assignment Instructions (max 18 points)

**Assignment points**, for which you can earn **18 points** for thorough completion:
  * Load the data from the `train.csv` file into the notebook. Divide the data into subsets that will be used for training, model comparison, and final model performance prediction.
  * Conduct a basic data exploration and discuss your observations. Display some of the images as well.
  * Construct and train several variants of a feedforward neural network model. Within the computational possibilities:
      * Comment on the suitability of the given model for the task.
      * Experiment with different depths and sizes of layers.
      * Experiment with data standardization/normalization.
      * Experiment with different optimization methods.
      * Experiment with various regularization techniques.
      * Always properly comment on the obtained results.

  * Construct a convolutional neural network model. Within the computational possibilities:
      * Comment on the suitability of the given model for the task.
      * Experiment with different depths and sizes of layers.
      * Experiment with data standardization/normalization.
      * Experiment with different optimization methods.
      * Experiment with various regularization techniques.
      * Always properly comment on the obtained results.
    
  * From all the tested options, choose the final model and estimate the accuracy you can expect on new data that you have not had access to before.
  
  * Finally, load the evaluation data from the `evaluate.csv` file. Use the final model to calculate predictions for this data (the target variable is not included). Create a `results.csv` file, in which the obtained predictions are saved in the **label** column and the identifiers in the **ID** column. Submit this file as well (save it in the project alongside the notebook).
   
   * Sample of the first few lines of the `results.csv` file:
  
ID,label

0,0

1,1


## Evaluation Part (max 7 points)
You can earn up to **7 points** for the accuracy of your submitted predictions for the evaluation set.

Denoting $A$ as the accuracy you achieved, rounded to 2 decimal places, the final points accumulate according to the following rules:
* if $A \geq 0.80$ you receive +1 point
* if $A \geq 0.83$ you receive +1 point
* if $A \geq 0.86$ you receive +1 point
* if $A \geq 0.87$ you receive +1 point
* if $A \geq 0.88$ you receive +1 point
* if $A \geq 0.89$ you receive +1 point
* if $A \geq 0.90$ you receive +1 point

**Example:** If your accuracy is 0.856, then A = 0.86 and you will receive 3 points.

**Results:** The final model's accuracy equals 0.9
