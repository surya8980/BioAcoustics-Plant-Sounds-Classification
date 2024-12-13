A dataset of audio files was prepared by merging audio recordings with identical ID into a 
single file. This merging combines fragmented recordings into meaningful units reducing 
redundancy. This was followed by preprocessing the .wav files such as resampling to a 
specified sampling rate and normalising amplitude to maintain uniformity. 
16 
 
The audio signals were then transformed into frequency domain from time domain. In the later 
stage, Short-Time Fourier transform (STFT) was used to generate Spectrograms, a visual 
representation of these transformed signals. These act as the inputs for Convolutional Neural 
Networks (CNN). To train the model with the uniform images, image augmentation techniques 
were applied to increase the diversity of the training dataset. It is not so sure that every 
spectrogram has the same level of brightness and other features. Techniques like rotation, 
scaling introduce variations that help the model generalise better to different levels. Then every 
image is resized into the model's input shape (128 x 128 x 3). A CNN is built by adding 
Convolutional layers followed by Batch Normalization and Max pooling layer. Adam 
Optimizer was used and categorical loss entropy and accuracy were monitored by setting 
verbose to 1. Early stopping was set to monitor validation loss with a patience level of 5.
