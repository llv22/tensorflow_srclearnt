# MNIST with tensorboard

## 1. How to Run
```bash
# in the root folder of source learning
# to avoid issue from source code ImportError: Could not import tensorflow. Do not import tensorflow from its source directory; change directory to outside the TensorFlow source tree, and relaunch your Python interpreter from there.
cd tensorflow/examples/tutorials
python mnist/mnist_with_summaries.py
```

this will generate log in /tmp/minist/logs, to visualize it, which requires to lanuch tensorboard. **Tensorflow change the implementation, so use tensorboard --logdir=/tmp/tensorflow/mnist/logs/mnist_with_summaries as your logging folder**
```bash
tensorboard --logdir=/tmp/tensorflow/mnist/logs/mnist_with_summaries
# TensorBoard 1.13.0a20181126 at http://cnpvgl903653:6006 (Press CTRL+C to quit)
```
## 2. Issue - https://stackoverflow.com/questions/14547631/python-locale-error-unsupported-locale-setting
```bash
# locale.Error: unsupported locale setting
export LC_ALL="en_US.UTF-8"
export LC_CTYPE="en_US.UTF-8"
sudo dpkg-reconfigure locales
```
generate locale as follow:
```bash
Generating locales (this might take a while)...
  en_AG.UTF-8... done
  en_AU.UTF-8... done
  en_BW.UTF-8... done
  en_CA.UTF-8... done
  en_DK.UTF-8... done
  en_GB.UTF-8... done
  en_HK.UTF-8... done
  en_IE.UTF-8... done
  en_IN.UTF-8... done
  en_NG.UTF-8... done
  en_NZ.UTF-8... done
  en_PH.UTF-8... done
  en_SG.UTF-8... done
  en_US.UTF-8... done
  en_ZA.UTF-8... done
  en_ZM.UTF-8... done
  en_ZW.UTF-8... done
  he_IL.UTF-8... done
```

## 3. Enjoying Code
