# Cyberlabs-MNIST-Challenge
This is a digit classification challenge for Cyberlabs


## What's this about?

The challenge is to make a classifier capable of differentiating the digits 0 and 5 of using the MNIST dataset.

## How did I did it?

Some resources were given such as the [fast.ai book](https://github.com/fastai/fastbook), this is a collection of jupyter notebooks that introduce deep learning, fast.ai, and Pytorch. The notebook that introduces MNIST and digit classification is this one [fast.ai MNIST](https://github.com/fastai/fastbook/blob/master/04_mnist_basics.ipynb).

Now, I don't have any experience training a neural network and the code under the hood, this was the first time, but the resources are really good and with a good math foundation it's sort of intuitive. 

### Approach

 The fast.ai book uses the fastbook library, it makes things such as data preparation easy, but I decided to use Pytorch to download the data, now this was quite a challenge, as the data must be transformed, and in this case it must be filtered in order to get only the digits of interest, this discussion helped with the [filtering](https://discuss.pytorch.org/t/how-to-use-one-class-of-number-in-mnist/26276/19). After organizing and filtering the data, I applied the method that fast.ai uses in the MNIST book, which consists in a linear classifier from scratch, that shows the logic under the hood. Than a simple model was created, using the steps showed on the fast.ai book. 
 
Now as this was quite challenging for me, I did tried not use the fastbook library, but on the training section I didn't succeded on using Pytorch only, so the fast.ai functions ``Learner`` and ``fit()`` were used. 

#### Result
Using simple model and a linear the accuracy results went quite well, both models got similar results as shown in this image

![Accucary](https://github.com/AbeRodz/Cyberlabs-MNIST-Challenge/blob/main/image.png "Graph")


## How to use?

This challenge was made on Google Colab, so I recommend using Colab for testing it, just click on the open on colab button or use this link [colab](https://colab.research.google.com/github/AbeRodz/Cyberlabs-MNIST-Challenge/blob/main/Cyberlabs_Challenge.ipynb). Create a copy, otherwise colab won't let it run.

