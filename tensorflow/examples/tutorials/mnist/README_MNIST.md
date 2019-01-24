# MNIST with tensorboard

## 1. How to Run
```bash
# in the root folder of source learning
# to avoid issue from source code ImportError: Could not import tensorflow. Do not import tensorflow from its source directory; change directory to outside the TensorFlow source tree, and relaunch your Python interpreter from there.
cd tensorflow/examples/tutorials
python mnist/mnist_with_summaries.py
```

this will generate log in /tmp/minist/logs, to visualize it, which requires to lanuch tensorboard
```bash
tensorboard -logdir=/tmp/minist/logs/mnist_with_summaries
```