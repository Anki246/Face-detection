# Face-detection-using-OpenCV-and-pretrained-dnn-model

OpenCV version 3.3 and above have “deep neural networks” (dnn ) module.
This module supports a number of deep learning frameworks, including Caffe, TensorFlow, and Torch/PyTorch.
When using OpenCV’s deep neural network module with Caffe models, you’ll need two sets of files:

The .prototxt file(s) which define the model architecture (i.e., the layers themselves)
The .caffemodel file which contains the weights for the actual layers
Both files are required when using models trained using Caffe for deep learning.



TO run the face detector:
1) go to terminal and activate your virtual environment
2) Navigate to the path where the 'detect_faces.py' is located and run : 
      python detect_faces.py --image inputs/im1.jpg --prototxt pretrained_detector_model/deploy.prototxt \
      --model pretrained_detector_model/res10_300x300_ssd_iter_140000.caffemodel
      
3) change the -- image, --prototxt and --model path with your pathe where you have saved the model and inouts and hit enter.
4) output image will be saved in current working directory

you can try this model on your own images





Thanks to the hard work of Aleksandr Rybnikov and the other contributors to OpenCV’s dnn  module,
we can enjoy these more accurate OpenCV face detectors in our own applications.
