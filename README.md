# [Train an object detection model On Google Colab](https://www.dlology.com/blog/how-to-train-an-object-detection-model-easy-for-free/)


## How to Run

Simplest way: run [this Colab Notebook](https://colab.research.google.com/github/fuadkhairi/object_detection_demo/blob/master/tensorflow_object_detection_training_colab.ipynb).

### Install required libraries
`pip3 install -r requirements.txt`

## How to run inference on frozen TensorFlow graph

Requirements:
- `frozen_inference_graph.pb` Frozen TensorFlow object detection model downloaded from Colab after training. 
- `label_map.pbtxt` File used to map correct name for predicted class index downloaded from Colab after training.

Run the following Jupyter notebook locally.
```
local_inference_test.ipynb
```

## Original Unmodified Repository by Tony u can find here
[Original Repo](https://github.com/Tony607/object_detection_demo)


TensorFlow benchmark on cpu
```
python local_inference_test.py\
     --model ./models/frozen_inference_graph.pb\
     --img ./test/15.jpg\
     --cpu
```
