---
title: "Visual Foresight with a Local Dynamics Model"
date: 2022-07-21
---
**Abstract:** Model-free policy learning has been shown to be capable of learning manipulation policies which 
can solve long-time horizon tasks using single-step manipulation primitives. However, training these policies 
is a time-consuming process requiring large amounts of data. We propose the Local Dynamics Model (LDM) which 
efficiently learns the state-transition function for these manipulation primitives. By combining the LDM with 
model-free policy learning, we can learn policies which can solve complex manipulation tasks using one-step 
lookahead planning. We show that the LDM is both more sample-efficient and outperforms other model architectures. 
When combined with planning, we can outperform other model-based and model-free policies on several challenging 
manipulation tasks in simulation. 
