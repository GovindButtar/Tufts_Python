This TFlite interpreter comes from 
https://www.tensorflow.org/lite/guide/python

And the models come from running the download script found here:
https://github.com/tensorflow/examples/tree/master/lite/examples/image_classification/raspberry_pi

The file classify_picamera.py has been slightly  modified to have a no preview mode
Instead of writing the label onto the camera output, it will print to the command line.

Run as follows:
python3 /home/jupyter/tflite/tflite_examples/lite/examples/image_classification/raspberry_pi/classify_picamera.py \
  --model /home/jupyter/tflite/tflite_models/mobilenet_v1_1.0_224_quant.tflite \
  --labels /home/jupyter/tflite/tflite_models/labels_mobilenet_quant_v1_224.txt \
  --preview no \
  --confidence 0.7

