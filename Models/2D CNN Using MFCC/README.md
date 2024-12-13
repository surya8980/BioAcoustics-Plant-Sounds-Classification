Mel Frequency Cepstral Coefficients (MFCC) were employed to transform the raw audio file into a sample containing the features of a particular wav file. These carry the numerical values that present in Frequency vs Time Spectrum.  

<p align="center">
  <img width="629" alt="{D9DD071B-FF9B-4779-82BB-8349012DF61A}" src="https://github.com/user-attachments/assets/05c650a6-5ad8-49de-a05d-c0e6136f1282" />
  <img width="629" alt="{43BF9E53-991B-4214-9D70-E185925FD4E8}" src="https://github.com/user-attachments/assets/9abc0e4e-191f-4874-91d6-c99de256937a" />
  <img width="629" alt="{BE5B2509-1D1F-4EFB-BD19-84F58004B265}" src="https://github.com/user-attachments/assets/78340d18-8da9-404f-859f-774f37b3653f" />
</p>


Based on these plots, MFCCs were calculated and stored in a 2D array. This 2D is similar to a 
grayscale image. This is fed as input to a customized CNN which is built from scratch. A 
sequential model was initialised. The first layer was a 2D Convolutional layer followed by a 
Max pooling layer and a dropout layer to prevent overfitting. The filter sizes were gradually 
increased from 32 to 64 and then to 128 to capture more hidden features. A Fully connected 
layer and a dense layer were added before the output layer. The output layer consists of 6 
classes with softmax function. 
