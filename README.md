# Imagewoof

## Dataset: Imagewoof 
Imagewoof is a subset of 10 classes from Imagenet that aren't so easy to classify, since they're all dog breeds. The breeds are: Australian terrier, Border terrier, Samoyed, Beagle, Shih-Tzu, English foxhound, Rhodesian ridgeback, Dingo, Golden retriever, Old English sheepdog.

## Training Details
### Model: ResNet 50
### Loss Function :  FlattenedLoss of CrossEntropyLoss
### Optimizer : ADAM
### Scheduler : One cycle Policy

## Results
### Image Size 128 (Random cropped) : Accuracy = 88.8%
<img src="https://github.com/orion29/Imagewoof/blob/main/Image/Unknown.png">

### Image Size 256 (Random cropped) : Accuracy = 93.0%
<img src="https://github.com/orion29/Imagewoof/blob/main/Image/Unknown-2.png">


