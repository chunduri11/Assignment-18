# Assignment-18
ShuffleNet, with tf eager mode

Tasks for this assignment:
1. Use **tfRecords** to load the data.
2. Used **tf eager mode** end to end.
3. applied **cutout** for data augmentation.
4. Achieved an accuracy of **80%(working to improve it)**, on evaluation data set.
5. Identified **50 miss-classified images** plotted them with its acutal label and predicted wrong lable. This will help us understand what leads to the confusion.


Modifications made to the original shuffleNet. Since the original shuffleNet is designed for ImageNet, we need to make some modifications for cifar10 or cifar100. This is the case with most of the modern DL Architectures.
1. Changed stride of first 3x3 convolution from a stride of two to one.
2. Removed the first max pool after the above convolution layer.
