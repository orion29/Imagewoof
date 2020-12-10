# Imagewoof

## Dataset: Imagewoof 
Imagewoof is a subset of 10 classes from Imagenet that aren't so easy to classify, since they're all dog breeds. The breeds are: Australian terrier, Border terrier, Samoyed, Beagle, Shih-Tzu, English foxhound, Rhodesian ridgeback, Dingo, Golden retriever, Old English sheepdog.


## Transforms Used

### Random Crop
Randomly crop an image to size

### Augment Transforms
<ul><li>Random flip</li>  
<li>Random rotation</li> 
<li>Random zoom </li>
<li>Perspective warping</li> 
<li>Changes in brightness and contrast</li> </ul> 


## Training Details

### Model: ResNet 50
ResNet-50 is a convolutional neural network that is 50 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database

### Loss Function :  FlattenedLoss of CrossEntropyLoss
Cross-entropy loss, or log loss, measures the performance of a classification model whose output is a probability value between 0 and 1. 

### Optimizer : ADAM
Adaptive Moment Estimation (Adam) is an optimizer that computes adaptive learning rates for each parameter. In addition to storing an exponentially decaying average of past squared gradients vt like RMSprop, Adam also keeps an exponentially decaying average of past gradients mt, similar to momentum.

### Scheduler : One cycle Policy
The 1cycle policy has three steps: We progressively increase our learning rate from base_lr to lr_max and at the same time we progressively decrease our momentum from mom_max to mom_min.

We do the exact opposite: we progressively decrease our learning rate from lr_max to lr_max/div_factor and at the same time we progressively increase our momentum from mom_min to mom_max.


## Results
### Image Size 128 (Random cropped) : Accuracy = 88.8%
<img src="https://github.com/orion29/Imagewoof/blob/main/Image/Unknown.png">

### Image Size 256 (Random cropped) : Accuracy = 93.0%
<img src="https://github.com/orion29/Imagewoof/blob/main/Image/Unknown-2.png">


