# Colorization-Model
Hyperparameter tuning

Hyperparameters Tuned:
Learning Rate (LR): 0.001, 0.0005, 0.0001
Batch Size: 32, 64
Number of Epochs: 30
Model Architecture: CNN with four convolutional layers.

Observations:
Experiment Results for Learning Rate:

LR = 0.001:
Accuracy plateaued at 68% after 15 epochs.
Overfitting observed after 12 epochs.
LR = 0.0005:
Optimal results with steady accuracy increase, reaching 72.5% at epoch 20.
Balanced precision and recall.
No overfitting detected.
LR = 0.0001:
Slow convergence, with only 65% accuracy after 20 epochs.
Increased training time with minimal performance gain.
Experiment Results for Batch Size:

Batch Size = 32:
Achieved 71.8% accuracy.
Slightly higher memory consumption but better generalization.
Batch Size = 64:
Achieved 72.5% accuracy (combined with LR = 0.0005).
Faster training with consistent results.
Recommended for this model setup.
Best Hyperparameter Combination:
Learning Rate (LR): 0.0005
Batch Size: 64
Epochs: 30
Model Architecture: 4-layer CNN
This combination provided the best balance between accuracy and training efficiency.

Reasoning for Best Parameters:
Learning Rate 0.0005: Prevented rapid overfitting, allowing gradual convergence.
Batch Size 64: Reduced variance in gradients, enabling faster training and better stability.
30 Epochs: Provided sufficient training without overfitting or resource wastage.


Overfitting was a concern with higher learning rates.
Smaller batch sizes (e.g., 32) offered slightly better generalization but increased training time.
Precision and recall metrics indicated good balance across classes with the chosen hyperparameters.

The training and evaluation demonstrated that the selected hyperparameters achieved a model accuracy of 72.5%.
