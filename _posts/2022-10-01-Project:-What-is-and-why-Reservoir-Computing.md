---
published: true
---
## The beginning of the story

I started to know about Reservoir computing (RC) at the third year of my PhD where I was trying to apply my research findings about dynamic skyrmions into a fancy application, eg. neuromorphic, AI, etc. The idea of RC attracted me because it perfectly merges the idea of complex neural network for a fancy task (just a demonstration) and a dynamic physical system, that could exsist almost everywhere (simply from a drop of water to any experimental systems in research labs)! This can actually be expanded to the idea of "computing", which happens at almost every moment and naturally in every systems (see the following pic where a bucket water was used to do pattern recognition for the tasks of XOR and spoken digit recognition, see also original paper: [Pattern recognition in a bucket](https://link.springer.com/chapter/10.1007/978-3-540-39432-7_63)).

![_config.yml]({{ site.baseurl }}/images/water bucket.png){: height="350px" width="auto"}

## What is RC?

There are many research articles, thesis and tutorials that talk about RC ([Reservoir computing approaches to recurrent neural network training](https://amygdala.psychdept.arizona.edu/CompNeuro/Readings/week13/Lukosevicius-Jaeger+Reservoir-computing-recurrent-neural-network+CompSciRev+2019.pdf), [Hands-on reservoir computing: a tutorial for practical implementation](https://iopscience.iop.org/article/10.1088/2634-4386/ac7db7/pdf), [Recent advances in physical reservoir computing: A review](https://arxiv.org/pdf/1808.04962.pdf), [Theory and Modeling of Complex Nonlinear Delay Dynamics Applied to Neuromorphic Computing](https://hal.archives-ouvertes.fr/tel-01591441/file/PhD_thesis-Penkovsky-arch.pdf)). RC was firstly proposed to solve the problems that Recurrent Neural Network training usually met. More specifically, traditional way of training RNN is based on the gradient descent method (In RNN, it is called back-propagation through time, BPTT, because the recurrent modual can be unfolded through time to become a feed forward neural network). However, this method fails when the number of time steps (depths) is very large because the error terms to calculate the gradient can be either exploded or vanished during the multiplication of each time steps according to the chain rule. That's why researchers proposed that instead of facing training problems, why not just keep the recurrent modual untrained 


The general framework of RC was first developed in early 2000-s independently by several
research groups: bearing a name of LSMs (liquid state machines) by the group of Maass [96],
the name of ESNs (echo state networks) by the team of Jaeger [97], and of backpropagationdecorrelation
(BPDC) by Steil [98]. The name reservoir computing serves as an umbrella term
emcompassing those approaches by illustrating the idea where the “reservoir” part of the processing
system is preexisting (even randomly generated) and remains unchanged, and only the
readout component is trained.


![_config.yml]({{ site.baseurl }}/images/RNN and RC2.png){: height="500px" width="auto"}


## Why RC is considered as "Brain-inspired"?



## Is there any real industrial-level applications of RC?


## Limitations of RC method



## Ongoing research and future of RC
talks about next generation of RC


References:
For someone who wants to know more about theoretical basis of RC
-
