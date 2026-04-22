# Deep Learning: CNN architectures {-}

This notebook is adapted from a Deep Learning course assignment. It involves training and testing the a CNN for an image classification task. We will go through the process of loading data, preprocessing images, building the CNN model, evaluating its performance, and discussing some relevant questions. Particularly,

1.  **Coding tasks:** 

    1.1 Implement a CNN architecture selected from the TensorFlow Keras Applications library (from the provided list https://www.tensorflow.org/api_docs/python/tf/keras/applications, excluding VGG16 and VGG19).  

    1.2 Train the selected CNN and evaluate its performance on the image classification task using appropriate evaluation metrics.  
    
    1.3 Enhance the model by introducing architectural modifications such as skip connections or by tuning layer level hyperparameters to improve performance.  

    1.4 Train and evaluate the enhanced model on the test dataset.

    1.5 Provide analysis and observations explaining how the applied modifications affected the model’s performance and behavior.  

2.  **Open discussion questions:** 

    2.1 When choosing a CNN architecture from the TensorFlow Keras library, what factors should be considered, such as model depth, number of parameters, and expected performance on the given dataset, and why might some architectures be more suitable than others for this specific image classification task?  

    2.2 During the data loading and preprocessing stage, in your opinion, what types of preprocessing steps are most important for image classification tasks, and how can improper preprocessing negatively affect the training stability and final performance of a CNN model?  

    2.3 After training the selected CNN model, how should different evaluation metrics such as accuracy, precision, recall, or confusion matrix be interpreted together to obtain a more complete understanding of the model’s strengths and weaknesses?  

    2.4 When introducing architectural modifications such as skip connections, what problems in deep neural networks are these modifications designed to solve, and how do they conceptually change the way information flows through the model?  

    2.5 From a broader perspective, what lessons can be learned from this assignment about the iterative nature of deep learning model development? Discuss why building an effective model typically requires repeated cycles of data preparation, model design, training, evaluation, and refinement rather than a single linear process.  

The dataset we will be working on is The CIFAR-10. This dataset consists of 60,000 32x32 colour images in 10 classes, with 6,000 images per class. There are 50,000 training images and 10,000 test images.
