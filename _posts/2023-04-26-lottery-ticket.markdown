---
layout: post
title:  "Lottery ticket hypothesis and its current state"
date:   2023-04-26
categories: meetings
---

In this meeting together with Jonathan Frankle we talked about famous lottery ticket hypothesis and how the research on sparsity developed since first appearance of the paper.
Some key takeaways from the discussion are:
- Pruning is done for training - not for optimality of the inference. So there is always a retraining phase that is supposed to gain good results.
- Initialization is critical - one needs to retain the initialization of the not pruned model, because otherwise the performance will not be reproduced.
- On MNIST one can reduce amount of weights till 3.6 percent of the initial amount while keeping same accuracy.
- Random subnetworks cannot train to the same accuracy, so pruning should be done in a valid way. 
- Adding noise during training can affect pruning that should be done - this might be an exciting new research direction.
- Early behaviour in the training is important, what learning rate was used there is important - this connects to the instability of the training, i.e., appearance of a linear barrier in the loss (bad performance of the averaged model).
- This line of research did not really affect the way networks should be trained, but led to multiple new insights of the inner workings of deep learning training.

You can find the (similar) talk [here](https://youtu.be/dYKiDwUEbCM).