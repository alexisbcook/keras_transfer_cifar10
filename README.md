[//]: # (Image References)

[image1]: ./images/tsne.png "t-SNE"

# Keras Transfer Learning on CIFAR-10

In the Jupyter notebook for this repository, I begin by calculating the bottleneck features for the [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) dataset.

These features are then visualized with a [Barnes-Hut implementation of t-SNE](http://lvdmaaten.github.io/tsne/), which is the fastest t-SNE implementation to date.  

For Python >= 3.5, this implementation can be installed by running

```
pip install git+https://github.com/alexisbcook/tsne.git
```

The bottleneck features are then fed to a shallow CNN for image classification.  The model attains a test accuracy of 82.68%.

![t-SNE][image1]