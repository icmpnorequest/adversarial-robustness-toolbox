# Adversarial Robustness Toolbox examples

[cifar_adversarial_training.py](cifar_adversarial_training.py)

Trains a convolutional neural network on the CIFAR-10 dataset, then generates adversarial images using the DeepFool attack and retrains the network on the training set augmented with the adversarial images.

[data_augmentation.py](data_augmentation.py)

This example shows how to use ART and Keras to perform adversarial training using data generators for CIFAR-10.

[mnist_cnn_fgsm.py](mnist_cnn_fgsm.py)

Trains a convolutional neural network on MNIST, then crafts FGSM attack examples on it.

[mnist_transferability.py](mnist_transferability.py)

Trains a convolutional neural network on the MNIST dataset using the Keras backend, then generates adversarial images using DeepFool and uses them to attack a convolutional neural network trained on MNIST using TensorFlow. This is to show how to perform a black-box attack: the attack never has access to the parameters of the TensorFlow model.

[mnist_poison_detection.py](mnist_poison_detection.py)

Generates a backdoor for MNIST dataset, then trains a convolutional neural network on the poisoned dataset and runs activation defence to find poison.

[data_poisoning_attack_svm.py](data_poisoning_attack_svm.py)

Perform data poisoning attack on the training labels, poison 40% of the training labels. Calculate and compare the result after poisoning.

<br> </br>

## Using Jupyter Notebooks to run ART

We have also created a sample Jupyter notebook in [Fabric for Deep Learning](https://github.com/IBM/FfDL) repository which shows you how to launch training using FfDL, and then invoke ART to find model vulnerabilities. Fabric for Deep Learning (FfDL, pronounced fiddle) is a Deep Learning Platform offering TensorFlow, Caffe, PyTorch etc. as a Service on Kubernetes

Find more details in the [code pattern here](https://developer.ibm.com/code/patterns/integrate-adversarial-attacks-model-training-pipeline/).
