# Plant Stress Classification using Ultrasonic Airborne Sounds  
# **Approach**  
**1.SVM Baseline Classifier:**
- The SVM model was tested using every pair of groups (e.g., drought-stressed, cut, control) to check for data balance and assess its utility for classification.
- The SVM was trained using a linear kernel and included feature scaling to normalize the features before training.
- The model's accuracy was computed to evaluate the dataset's balance and usefulness for further classification tasks.

**2.Convolutional Neural Network (CNN):**

- CNNs are a powerful tool for automatic feature extraction and classification, especially for tasks involving image or sound data.
- CNNs are particularly suitable for this project due to their ability to identify complex patterns without human supervision and prevent overfitting using weight sharing.
- The model will be designed to classify plant conditions based on ultrasonic airborne sound data.

# CNN Model Architecture
Despite the evolution of deep learning models, CNNs remain one of the most widely used and effective models, especially in fields like image recognition and speech recognition.

**Key Advantages of CNN:**
- Automatic Feature Extraction: CNNs do not require manual feature engineering and can automatically identify relevant patterns in the data.
- Weight Sharing: This helps in preventing overfitting and improves the model's ability to generalize to new data.
- Local Connections: CNNs leverage local connections between neurons, making them particularly well-suited for processing 2D data structures, such as visual or acoustic signals.
# Why CNN for This Task?
- CNNs are inspired by the way the visual cortex in animals, such as cats, processes information. By using parameter sharing and sparse interactions, CNNs can efficiently process large datasets and automatically learn the important features for classification.
- Compared to traditional Fully Connected (FC) networks, CNNs are more efficient because they exploit the 2D nature of the input data (in this case, ultrasonic sounds).
- This approach significantly reduces the number of parameters, making the model easier to train and less prone to overfitting.
