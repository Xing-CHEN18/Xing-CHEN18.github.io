---
published: false
---

When talking about reservoir computing, one must mention that the reservoir's main requirements are nonlinearity and a memory effect, also known as the 'echo state property' in the context of Echo State Networks (see more in one of my other blog: ([What is and why reservoir computing](https://xing-chen18.github.io/Project-What-is-and-why-Reservoir-Computing/)). But why it isn't a system has certain memory effect must also have nonlinearity? Intuitively, Nonlinear systems often exhibit complex behaviors that are sensitive to initial conditions, such as chaos. Since memory effects introduce a form of complexity— where the output depends not just on the current input but also on past inputs— it can be easy to conflate this complexity with nonlinearity.

Let's break is up firstly by uderstanding the concept of nonlinearity and memory effect:

**Nonlinearity**: Nonlinear dynamics within the reservoir allow the system to project the input data into a high-dimensional space, creating complex temporal patterns that can be linearly separable. This is crucial for the learning process because it allows the network to handle tasks that are fundamentally nonlinear in nature, which most real-world tasks are.

**Memory Effect**: The reservoir must possess a memory effect to retain information about past inputs over some time horizon. This is necessary for processing sequences and time-series data where the output depends on the history of inputs, not just the current one.