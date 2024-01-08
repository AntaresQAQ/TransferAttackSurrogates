# TransferAttackSurrogates

The implementation of our IEEE S&P 2024 paper "Why Does Little Robustness Help? A Further Step Towards Understanding Adversarial Transferability"



## Abstract
Adversarial examples for deep neural networks (DNNs) have been shown to be transferable: examples that successfully fool one white-box surrogate model can also deceive other black-box models with different architectures. Although a bunch of empirical studies have provided guidance on generating highly transferable adversarial examples, many of these findings fail to be well explained and even lead to confusing or inconsistent advice for practical use. 

In this paper, we take a further step towards understanding adversarial transferability, with a particular focus on surrogate aspects. Starting from the intriguing “little robustness” phenomenon, where models adversarially trained with mildly perturbed adversarial samples can serve as better surrogates for transfer attacks, we attribute it to a trade-off between two dominant factors: model smoothness and gradient similarity. Our research focuses on their joint effects on transferability, rather than demonstrating the separate relationships alone. Through a combination of theoretical and empirical analyses, we hypothesize that the data distribution shift induced by off manifold samples in adversarial training is the reason that impairs gradient similarity. 

Building on these insights, we further explore the impacts of prevalent data augmentation and gradient regularization on transferability and analyze how the trade-off manifests in various training methods, thus building a comprehensive blueprint for the regulation mechanisms behind transferability. Finally, we provide a general route for constructing superior surrogates to boost transferability, which optimizes both model smoothness and gradient similarity simultaneously, e.g., the combination of input gradient regularization and sharpnessaware minimization (SAM), validated by extensive experiments. In summary, we call for attention to the united impacts of these two factors for launching effective transfer attacks, rather than optimizing one while ignoring the other, and emphasize the crucial role of manipulating surrogate models.
