---
published: true
---

When talking about reservoir computing, one must mention that the reservoir's main requirements are nonlinearity and a memory effect, also known as the 'echo state property' in the context of Echo State Networks (see more in one of my other blog: ([What is and why reservoir computing](https://xing-chen18.github.io/Project-What-is-and-why-Reservoir-Computing/)). But why it isn't a system has certain memory effect must also have nonlinearity? Intuitively, Nonlinear systems often exhibit complex behaviors that are sensitive to initial conditions, such as chaos. Since memory effects introduce a form of complexity— where the output depends not just on the current input but also on past inputs— it can be easy to conflate this complexity with nonlinearity.

Let's break is up firstly by uderstanding the concept of nonlinearity and memory effect:

**Nonlinearity**: Nonlinear dynamics within the reservoir allow the system to project the input data into a high-dimensional space, creating complex temporal patterns that can be linearly separable. This is crucial for the learning process because it allows the network to handle tasks that are fundamentally nonlinear in nature, which most real-world tasks are.

**Memory Effect**: The reservoir must possess a memory effect to retain information about past inputs over some time horizon. This is necessary for processing sequences and time-series data where the output depends on the history of inputs, not just the current one.

To address whether systems with memory effects naturally exhibit nonlinearity, it's important to note that memory effects and nonlinearity are related but distinct properties:

-A system has a memory effect if its output at any time depends not only on the current input but also on past inputs.
-A system is nonlinear if the relationship between its input and output cannot be described by a linear equation.

While many systems with memory are nonlinear, this is not a strict requirement. For example:

A Linear Time-Invariant (LTI) system is defined by linearity and time-invariance, and it can have a memory. For instance, a simple RC circuit (a resistor and capacitor in series) can act as a linear filter that has memory (the voltage across the capacitor depends on the history of the input voltage). The system's response can be fully described by a linear differential equation.

A Linear Time-Varying (LTV) system also can have memory and might have coefficients that change over time, but still maintains linearity in terms of the input-output relationship. An example might be a system whose resistance changes over time in a predictable manner.

Nonlinear systems, however, are characterized by equations where the output is not proportional to the input. The behavior of such systems can be much more complex and less predictable than linear systems.



