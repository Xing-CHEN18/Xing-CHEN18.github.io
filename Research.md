


Research Overview

- ## Advancing the Forward-Forward Algorithm

**Related fields**: Slef-supervised learning, un-supervised learning, Noise contrastive Learning, Bio-inspired learning, local learning, Neuromorphic algorithm

**Introduction**: The Forward-Forward Algorithm, as conceptualized by Geoffrey Hinton, is a novel approach to learning in neural networks. This learning method is particularly distinctive because it replaces the traditional forward and backward passes of backpropagation—fundamental to deep learning— with two forward passes. This project can be presented as a step towards more energy-efficient and potentially biologically realistic forms of learning in artificial neural networks. 

<p align="center">
  <img alt="img-name" src="{{ site.baseurl }}/images/SCFF.png" height="auto" width="auto">
    <em>Comparison of FF, Contrastive Learning and SCFF (our method)</em>
</p>

To learn more about the details, I would recommend watching his interview, or my post for a general intro: [Introduction Of The Forward Forward Method By Geoffrey Hilton](https://xing-chen18.github.io/Project-Introduction-of-the-forward-forward-method-by-Geoffrey-Hilton/)

**My Work**: I have developed an advanced method of generating negative data that diverges from and improves upon Geoffrey Hinton's initial Forward-Forward Algorithm framework. My approach has been tested on diverse datasets, ranging from vison (MNIST, CIFAR, STL-10 (a few number of labeled data alongside a large amount of unlabeled data)) to audio (FSDD dataset) tasks. The approach has not only achieved remarkable accuracy but also surpassed the performance benchmarks set by existing unsupervised local learning algorithms.

**Impact**: Improving machine learning models' interpretability. The implications extend to real-world applications, including but not limited to, enhanced computer vision systems, more efficient natural language processors, etc.

**Publication and code**: Manuscript currently available at arXiv: [Self-Contrastive Forward-Forward Algorithm](https://arxiv.org/abs/2409.11593). Code is available at [Github repo](https://github.com/neurophysics-cnrsthales/contrastive-forward-forward).


- ## Neural Ordinary Differential Equations for modeling time series data

**Related fields**: Residual Network, Differential Equations, Time series forcasting

**Introduction**: This study addresses the gap in applying artificial intelligence to discover the complete differential equations governing physical experiments. It focuses on the domain of spintronics, where the behavior of devices underpins future technological advancements.

<p align="center">
  <img alt="img-name" src="{{ site.baseurl }}/images/NODE.PNG" height="auto" width="auto">
    <em>Design of the network architecture and test prediction</em>
</p>

**My Contribution**: I led the initiative to adapt Neural Ordinary Differential Equations to spintronics' unique constraints, involving few outputs, multiple inputs, and internal parameters. Our model, trained on minimal data, successfully predicted spintronic devices' behaviors with remarkable accuracy and efficiency.

**Impact**: Our approach demonstrated an over 200-fold acceleration in simulation time compared to traditional methods, predicting the response of experimental spintronic nano-oscillators effectively. It stands to significantly speed up the development process in spintronics and potentially other areas involving dynamic electronic devices.

**Reflection/Future Work**: The promising results from Neural ODEs in spintronics suggest a disruptive tool for rapid and accurate modeling, complementing time-intensive micromagnetic simulations. Looking ahead, we aim to generalize this approach to a broader range of electronic devices, optimizing the functionality and efficiency of next-generation technologies.

**Publication and code**: [Forecasting the outcome of spintronic experiments with neural ordinary differential equations](https://www.nature.com/articles/s41467-022-28571-7), _Nat Commun 13, 1016 (2022)_.

- ## Reservoir computing for modeling time series data

**Related field**: Echo state network, Ridge regression

**Introduction**: This work explores the implementation of reservoir computing (RC) systems, a subset of neuromorphic computing, which are particularly efficient for processing temporal and sequential information. These systems utilize a network of nonlinear nodes for rapid and stable learning, significantly reducing computational costs compared to traditional recurrent neural networks (RNNs). For more info about RC, pls check my previous posts if it interests you: [Project: What Is And Why Reservoir Computing](https://xing-chen18.github.io/Project-What-is-and-why-Reservoir-Computing/), [Memory and Nonlinearity in Reservoir Computing](https://xing-chen18.github.io/Project-Memory-and-Nonlinearity-in-Reservoir-Computing/)

<p align="center">
  <img alt="img-name" src="{{ site.baseurl }}/images/NC_reservoir.PNG" height="auto" width="auto">
    <em>Reservoir network and its ability to predict chaotic time series</em>
</p>

**My Contribution**: I contributed to the design of reservoir computing experiments and optimization of the algorithms for train the network.

**Impact**: This work successfully demonstrated the functionality of RC system in waveform classification and time series prediction tasks, achieving a recognition rate of 99.3% and a normalized root mean square error of 0.2, respectively. These results highlight the potential of our system in developing low-power, highly efficient neuromorphic computing systems, paving the way for advanced spintronic applications.

**Reflection/Future Work**: This research represents a significant step towards leveraging magneto-electro-ferroelastic tunability for neuromorphic computing. Going forward, the aim is to extend these concepts to more complex applications and further optimize the system for real-world neuromorphic computing challenges.

**Publication and code**: [Experimental demonstration of a skyrmion-enhanced strain-mediated physical reservoir computing system](https://www.nature.com/articles/s41467-023-39207-9), _Nat Commun 14, 3434 (2023)_. Code is available at [Github repo](https://github.com/Xing-CHEN18/NeuralODEs_for_physics).

- ## Micromagnetic simulations for modeling magnetic materials

**Related fields**: Partial differential equations, Finite Difference Method, Numerical analysis

**Introduction**: Just as weather simulations predict the weather, micromagnetic simulations forecast the behavior of magnetic materials, which are crucial in many technologies around us — from the hard drives storing our precious memories to the sensors in our smartphones.  To know more about Micromagnetic simulations, have a look at my previous post: [How does FFT helps in micromagnetic simulations](https://xing-chen18.github.io/My-PhD/)

<p align="center">
  <img alt="img-name" src="{{ site.baseurl }}/images/mics.png" height="auto" width="auto">
    <em>Left: Scales in micromagnetism. Right: Magnetic phenomenon under certain conditions </em>
</p>

**My work**: I worked on several projects during my phd about modeling and simulations of the magnetic materials to explore their dynamical characteristics under external sources (e.g., current, voltage, magnetic field). The mathematical approaches being used included partial differential equations, ordinary differential equations, Finite Difference Method, Monte Carlo Simulations, Fourier Transforms .etc.

**Selected publications**: 

- [A compact skyrmionic leaky–integrate–fire spiking neuron device](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=_1rFPswAAAAJ&citation_for_view=_1rFPswAAAAJ:u5HHmVD_uO8C), 	_Nanoscale, 2018,10, 6139-6146_.

- [Skyrmion dynamics in width-varying nanotracks and implications for skyrmionic applications](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=_1rFPswAAAAJ&citation_for_view=_1rFPswAAAAJ:2osOgNQ5qMEC), _Appl. Phys. Lett. 111, 202406 (2017)_.

- [Magnetic skyrmion spectrum under voltage excitation and its linear modulation](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=_1rFPswAAAAJ&citation_for_view=_1rFPswAAAAJ:Y0pCki6q_DkC), _Phys. Rev. Applied 12, 024008_.


## List of my posts
_I want to know more about other things_ 

- [Project: Introduction Of The Forward Forward Method By Geoffrey Hilton](https://xing-chen18.github.io/Project-Introduction-of-the-forward-forward-method-by-Geoffrey-Hilton/)

- [Project: What Is And Why Reservoir Computing](https://xing-chen18.github.io/Project-What-is-and-why-Reservoir-Computing/)

- [Project: How does FFT helps in micromagnetic simulations](https://xing-chen18.github.io/My-PhD/)

- [Daily: Why Not Drink Hot Water From Tap](https://xing-chen18.github.io/Daily-Turning-Up-the-Heat-Why-You-Rethink-Drinking-Warm-Tap-Water/)

- [Know How: Git Usage](https://xing-chen18.github.io/know-how-Git-usage/)

- [Daily: How Does A Ticket Work](https://xing-chen18.github.io/Daily-How-does-a-ticket-work/)

- [Daily: Why Eu Countries Do Not Use Qr Code Payment As China Does](https://xing-chen18.github.io/Daily-Why-Eu-countries-do-not-use-QR-code-payment-as-China-does/)

- [Daily: Tunnel Vision](https://xing-chen18.github.io/Daily-Tunnel-vision/)

- [Daily: You Are Ready When You Are Ready](https://xing-chen18.github.io/Daily-You-are-ready-when-you-are-ready/)
