---
layout: post
title:  "Exploring Generalization in Deep Learning"
date:   2022-01-18
categories: meetings
---

In this meeting we discussed the paper by B. Neyshabur et al. "Exploring Generalization in Deep Learning".
This paper was published at NeurIPS 2017.

Interesting points:
- Are there any in depth analysis of the Lipschitz constraint generalization explanation for deep neural networks?
- Are there generalization measures that are suited for OOD setup? Or the iid requirement is always there (as follows from ERM formulation)
- Does the “confusion set injection” experimental setup contradict iid assumption or not?
- Most probably, is it is trained till real 0 loss on the clean part of the training data, then it should not contradict. But it is unclear if it is the case in the paper.
- Why double descent does not appear in the MNIST-width experiments?
- Important to keep in mind the goal of the “generalization measure” - since non-uniform for one selected architecture measure cannot for example help to choose better or worse architecture.
- Why rescaling for norm-based measures is done exactly with the difference between maximal prediction and the next largest?
- To take into account “certainty” of the prediction that basically reflects the margin between classes


You can find the presentation that was held [here](https://docs.google.com/presentation/d/1lKgOmQV1zQjHd_VmBTA0fG_Sn7hlTUof/edit?usp=share_link&ouid=103183581597903717528&rtpof=true&sd=true).