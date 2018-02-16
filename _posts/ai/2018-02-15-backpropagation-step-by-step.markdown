---
layout: post
title:  "Backpropagation Step by Step"
date:   2018-02-15 14:30:00
categories: ai
description: Backpropagation is a technique used for training neural network. There are many resources explaining the technique, but this post will explain backpropagation with concrete example in a very detailed colorful steps. 
---


<p style="text-align: justify;">
	
	<a href="http://hmkcode.github.io/images/ai/backpropagation.png">
		<img class="size-full wp-image-315 aligncenter" src="http://hmkcode.github.io/images/ai/backpropagation.png" alt="get-location" />
	</a>
	
	If you are trying to understand or build your own neural network, then you will definitely need to understand how to train your network.
	Backpropagation is a commonly used technique for training neural network. There are many resources explaining the technique, 
	but this post will explain backpropagation with concrete example in a very detailed colorful steps.
</p>

## Overview

In this post, we will use a neural network with two inputs, two hidden neurons and one output neuron. 

![android-tabs]({{ "http://hmkcode.github.io/images/ai/nn1.png" | absolute_url }})




## Weights, weights, weights

Neural network training is about finding weights that minimize prediction error. We usually start our training with a set of randomly generated weights.Then, backpropagation is used to update the weights in an attempt to correctly map arbitrary inputs to outputs.

Our initial weights will be as following:
`w1 = 0.11`, `w2 = 0.21`, `w3 = 0.12`, `w4 = 0.08`, `w5 = 0.14` and `w6 = 0.15`

![bp_weights]({{ "http://hmkcode.github.io/images/ai/bp_weights.png" | absolute_url }})

## Training Set

We will use a training set that has two inputs and one output. Our data set has a single sample with `inputs=[2, 3]` and `output=[1]`.



### Source Code @ [GitHub](https://github.com/hmkcode/Android/tree/master/user-interface/android-swipe-views-tabs)
