# ASL Recognition

 Display asl handsigns infront of your webcam to have the nano determine what letter it represents

![add image descrition here](https://github.com/U4Shinez/Project1/blob/master/output.jpg)

## The Algorithm
The algorithm worked by taking 35 second videos at 30 fps of hand signs for each of the 26 letters in the alphabet. In total, each letter has 1050 photos. However, the algorithm, better known as imagenet, used only 80% of the photos (840 photos) to train itself. The dataset was ran through the model 35 times, which is known as epochs. Epochs help bring up the accuracy of the models identifcation the more you run your dataset through it. Next, we used a test image from the dataset to observe if the outputed resnet-18 model could identify correctly what letter the hand in the image represented; this was supplamented by an accuracy rating next to the letter in the top left of the output photo.

## Running this project
1. Install Jetson Inference Library
2. `imagenet.py --model=resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=labels.txt input output`

[View a video explanation here](video link)
