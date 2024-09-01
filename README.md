# STOCHASTIC-BATCH-GRADIENT
In deep learning, optimization algorithms use different gradient descent methods to update model parameters and minimize the loss function. Two common methods are Stochastic Gradient Descent (SGD) and Batch Gradient Descent. Here’s a brief overview of each:
Stochastic Gradient Descent (SGD)

    Overview: In SGD, the model parameters are updated using a single training example (or a very small subset) at a time.

    Process:
        Pick a random training example from the dataset.
        Compute the gradient of the loss function with respect to the parameters for this example.
        Update the parameters using this gradient.
        Repeat this process for many iterations or epochs.

    Advantages:
        Can handle large datasets since it processes one example (or a small batch) at a time.
        Often helps to escape local minima due to the noisy gradient updates.
        Can be more computationally efficient with large datasets.

    Disadvantages:
        The updates are noisy, which can make the convergence path erratic and slow.
        Requires careful tuning of the learning rate.

Batch Gradient Descent

    Overview: In Batch Gradient Descent, the model parameters are updated using the entire training dataset.

    Process:
        Compute the gradient of the loss function using the entire dataset.
        Update the parameters based on this gradient.
        Repeat this process for many iterations or epochs.

    Advantages:
        Provides a more accurate estimate of the gradient since it uses the entire dataset.
        The convergence path tends to be smoother compared to SGD.

    Disadvantages:
        Can be computationally expensive and memory-intensive, especially with large datasets.
        May get stuck in local minima or saddle points due to lack of noise in gradient estimates
