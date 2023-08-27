---
title: "Encoder-Decoder Image Captioning on COCO-2015 Dataset
collection: projects
type: "Undergraduate course"
permalink: /image_captioning/
---

This is a description of a teaching experience. You can use markdown like any other post.

Encoder
======
The encoder is either a custom convolutional network or the ResNet-50 pre-trained on ImageNet. 

For the custom model, we add a drop-out layer that randomly disable half of the hidden units to improve generalization. 
The embedding size of the network is switched to 512 from 300. 
In this way, we enlarge the number of unique orthogonal feature representations for the model vocabulary, so the network is able to generate captions with a wider range of words. 

Decoder
======
The decoder is a custom Long Short Term Memory network.

It is trained with teacher-forcing. That is, we feed each character of the label caption into the network. 

It generates captions deterministically or stochastically, with a temperature that enables a probability distribution according to the temperature value. 
A very small temperature parameter is almost deterministic. 
A large temperature would foster random words that has low occurrences. 

Example Output
======
---
title: "Best Custom-CNN Encoder-Decoder Performance"
excerpt: "Short description of portfolio item number 1<br/><img src='/images/500x300.png'>"
collection: portfolio
---

[Checkout Our Report](http://jingyuanhe1222.github.io/files/Image Captioning by Encoder-Decoder Structure.pdf)
