# MNIST with tensorboard

## 1. How to Run
```bash
# in the root folder of source learning
python tensorflow/examples/tutorials/mnist/mnist_with_summaries.py
```

this will generate log in /tmp/minist/logs, to visualize it, which requires to lanuch tensorboard
```bash
tensorboard -logdir=/tmp/minist/logs/mnist_with_summaries
```