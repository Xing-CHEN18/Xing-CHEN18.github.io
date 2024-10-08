---
published: true
---
## The beginning of the story

I started to know about Reservoir computing (RC) at the third year of my PhD where I was trying to apply my research findings about dynamic skyrmions into a fancy application, eg. neuromorphic, AI, etc. The idea of RC attracted me because it perfectly merges the idea of complex neural network for a fancy task (just a demonstration) and a dynamic physical system, that could exsist almost everywhere (simply from a drop of water to any experimental systems in research labs)! This can actually be expanded to the idea of "computing", which happens at almost every moment and naturally in every systems (see the following pic where a bucket water was used to do pattern recognition for the tasks of XOR and spoken digit recognition, see also original paper: [Pattern recognition in a bucket](https://link.springer.com/chapter/10.1007/978-3-540-39432-7_63)).

![_config.yml]({{ site.baseurl }}/images/water bucket.png)

## What is RC?

There are many research articles, thesis and tutorials that talk about RC ([Reservoir computing approaches to recurrent neural network training](https://amygdala.psychdept.arizona.edu/CompNeuro/Readings/week13/Lukosevicius-Jaeger+Reservoir-computing-recurrent-neural-network+CompSciRev+2019.pdf), [Hands-on reservoir computing: a tutorial for practical implementation](https://iopscience.iop.org/article/10.1088/2634-4386/ac7db7/pdf), [Recent advances in physical reservoir computing: A review](https://arxiv.org/pdf/1808.04962.pdf), [Theory and Modeling of Complex Nonlinear Delay Dynamics Applied to Neuromorphic Computing](https://hal.archives-ouvertes.fr/tel-01591441/file/PhD_thesis-Penkovsky-arch.pdf)). RC was firstly proposed to solve the problems that Recurrent Neural Network training usually met. More specifically, traditional way of training RNN is based on the gradient descent method (In RNN, it is called back-propagation through time, BPTT, because the recurrent modual can be unfolded through time to become a feed forward neural network). However, this method fails when the number of time steps (depths) is very large because the error terms to calculate the gradient can be either exploded or vanished during the multiplication at each time steps according to the chain rule. That's why researchers proposed that instead of facing training problems, why not just keep the recurrent modual untrained. This idea of RC was firstly develped by several research groups as [liquid state machines](https://direct.mit.edu/neco/article-abstract/14/11/2531/6650/Real-Time-Computing-Without-Stable-States-A-New), [echo state networks](https://www.ai.rug.nl/minds/uploads/EchoStatesTechRep.pdf) and [backpropagationdecorrelation](https://ieeexplore.ieee.org/document/1380039) in early 2000s. The name reservoir computing serves as an umbrella term emcompassing those approaches by illustrating the idea where the “reservoir” part of the processing system is preexisting (even randomly generated) and remains unchanged, and only the readout component is trained (see the pic below).

![_config.yml]({{ site.baseurl }}/images/RNN and RC2.png)


## Why RC is considered as "Brain-inspired"?

The computational approach of RC stands out as a brain-inspired framework to produce hardware neural networks and perform on-chip computation [Theory and Modeling of Complex Nonlinear Delay Dynamics Applied to Neuromorphic Computing](https://hal.archives-ouvertes.fr/tel-01591441/file/PhD_thesis-Penkovsky-arch.pdf). 
- Neural networks used for RC consist of a reservoir of randomly ordered nonlinear neurons, whose connections are not subject to training; this group of disordered, recurrent connected neurons behaves similarly to a cortical column in a biological neural system. An analogy is that the brain serves as a general-purpose “device” allowing to quickly adapt to new and unexpected situations. One of the possible explanations how such adaptability is possible could be the brain is a complex network. If it is very complex, some of the solution trajectories must already exist in the high-dimensional dynamics of such a system. The remaining learning procedure is rewiring the brain connections so that useful trajectories are amplified and not useful ones are suppressed.

- Another notable analogy between RC and the brain is their underlying memory hierarchy. Unlike conventional computers, the human brain has memory inseparable from computing units (neurons). RC tries to alleviate this discrepancy by including memory in the computation procedure.

## What is the advantages of RC & Is there any real industrial-level applications of RC?

Here are some advantages of Reservoir Computing:

_Training Efficiency_: One of the main benefits of RC is that training is typically much faster compared to traditional recurrent neural networks (RNNs) like LSTMs or GRUs. This is because only the output weights of the reservoir need to be trained, while the recurrent part remains fixed.

_Rich Dynamics with Sparse Connectivity_: The reservoir, even when sparsely connected, can exhibit a wide range of dynamic behaviors, allowing it to generate rich temporal representations of the input sequences.

_Avoidance of Gradient-based Issues_: Traditional RNNs can suffer from problems like the vanishing or exploding gradient. Because RC doesn't require gradient-based training for its recurrent part, it avoids these issues.

_Flexibility_: The reservoir can be implemented using various structures or even physical systems. This leads to applications in "physical reservoir computing", where physical processes, such as water waves or optical systems, act as reservoirs.

_Regularization_: The structure of RC naturally introduces a form of regularization, which can sometimes lead to better generalization on certain tasks.

_Adaptability_: Reservoir Computing can be applied to a variety of time series tasks without much change in the reservoir's structure.

As for industrial-level applications:

_Time Series Prediction_: This is one of the primary applications of RC. Industries with a lot of time series data (like finance, energy, or retail) can use RC for forecasting.

_Anomaly Detection_: In industries like manufacturing, RC can be used to detect anomalies in time series data, such as machine wear and tear or process disruptions.

_Robotics_: RC has been explored in robot control tasks, especially in scenarios that involve temporal patterns.

_Telecommunications_: RC has been researched for applications in channel equalization and signal processing.

_Physical Reservoir Computing_: As mentioned, there's growing interest in using physical processes as reservoirs. This has potential applications in areas like optical computing and other specialized computing architectures.

_Image classification_: Though not widely used, there are also some work exploring the power of RC for image recognition. For example, in the paper of [Reservoir Computing with Untrained Convolutional Neural Networks for Image Recognition](https://ieeexplore.ieee.org/document/8545471), where they propose a new method which combines reservoir computing with untrained convolutional neural networks. They use an untrained convolutional neural network to transform raw image data into a set of smaller feature maps in a preprocessing step of the reservoir computing. 


## Limitations of RC method

However, while RC has some advantages and has been applied in various domains, it hasn't seen as widespread industrial adoption as some other neural network architectures. This is partially due to the dominance and flexibility of other RNN architectures like LSTMs and GRUs, as well as the surge of Transformer-based models, which have achieved state-of-the-art performance on many tasks.

More specifically:

_Fixed Reservoir_: The reservoir in RC is typically not trained. While this speeds up training, it can also limit the performance of the network, especially if the reservoir's initial configuration isn't suitable for the task.

_Hyperparameter Sensitivity_: The performance of RC is often sensitive to the choice of hyperparameters, such as reservoir size, connectivity density, spectral radius, and input scaling. Finding the right set of hyperparameters can require a lot of trial and error.

_Scalability_: While RC is efficient in certain applications, especially those involving time series data, it might not scale as effectively for more complex tasks when compared to other architectures like LSTMs or GRUs.

_Memory Limitations_: Large reservoirs can require significant memory, which can become a bottleneck in some applications.

_Non-universality_: While traditional recurrent networks like LSTMs have demonstrated versatility across a wide range of tasks, RC's applicability can sometimes be more niche.

_Difficulty with Long Sequences_: Despite being a recurrent architecture, RC can sometimes struggle with very long sequences, especially if the reservoir is not sufficiently large or properly configured.

_Research Gap_: Compared to more mainstream neural network architectures, there's a smaller community working on RC, which means there might be fewer tools, pre-trained models, and resources available.

_Limited Transfer Learning_: One of the strengths of deep learning is the ability to transfer learned features from one task to another using pre-trained models. Given the fixed nature of the reservoir in RC, this kind of transfer learning is less straightforward.

_Physical Implementation Challenges_: While there's interest in physical reservoir computing (e.g., using optical systems or other physical processes as reservoirs), these can introduce challenges in terms of hardware implementation, stability, and reproducibility.

## Ongoing research and future of RC

_Physical Reservoirs_: There's growing interest in implementing reservoirs in physical systems, such as optical systems, water waves, or electronic circuits. These physical reservoirs can be incredibly fast and power-efficient, opening the door for real-time, low-power processing applications.

_Optimization of Hyperparameters_: Given the sensitivity of RC to hyperparameters, research into automated methods for optimizing these (e.g., using genetic algorithms or other search techniques) continues to be of interest.

_Deep Reservoirs_: While traditional RC typically employs a single reservoir layer, there's exploration into stacking multiple reservoirs to form a deep architecture, potentially improving the expressive power of the model.

_Training the Reservoir_: Although the reservoir is traditionally kept fixed, some research directions involve partially training or adapting the reservoir to better fit specific tasks, aiming to combine the best of traditional RNNs and RC.

_Hybrid Models_: Combining RC with other neural network architectures, such as convolutional layers for image data or transformers for sequence data, could harness the strengths of both worlds.

_Regularization and Stability_: Investigating techniques to improve the stability and generalization of RC, ensuring that the reservoir dynamics are rich yet controlled.

_Neuromorphic Implementations_: With the rise of neuromorphic computing, where hardware is designed to mimic the brain's neural structure, RC could play a role given its brain-inspired approach to processing temporal data.

_Large-scale Applications_: Exploring the scalability of RC to handle larger, more complex real-world applications, such as high-dimensional time series forecasting, large-scale robotics control, and more.

_Theory and Analysis_: Deepening the theoretical understanding of why and when RC works, drawing parallels to brain function, and studying the mathematical properties of reservoirs.

_Application in Edge Devices_: Given the efficiency of RC, there's potential for its application in edge devices where computational resources are limited but real-time processing is essential.

Also checkout the paper of [Next generation reservoir computing](https://www.nature.com/articles/s41467-021-25801-2) for further insights.


