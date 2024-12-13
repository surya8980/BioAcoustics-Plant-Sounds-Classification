# Residual CNN
After the Customized CNN results, some other models were explored to improve the model’s 
performance and challenges such as vanishing gradient. A Resnet variant was employed due 
to its architecture, with its residual connections which allows for efficient feature extraction 
from audio files converted into images in frequency domain. This enables the model to learn 
complex patterns tackling the vanishing gradient which leads to improved accuracy. MFCC 
from clean audio was extracted and Dataset was split into train, test,validation using train test 
split. A reshaped 2D array is fed as input to the RCNN. 
<p align = "center">
<img width="659" alt="{C8EB758A-6F40-4DFE-9488-DD90F3E2A48C}" src="https://github.com/user-attachments/assets/77603877-c86f-4e3a-b61a-ca119f13e6a6" />
</p>

