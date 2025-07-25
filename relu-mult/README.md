### ReLU(x)*ReLU(y) 

This fork has been created to explore if using _ReLU(x)*ReLU(y)_ activation functions taking two linear combinations on their inputs might bring further improvement.

This is following an idea mentioned on page 4 of _Programming Patterns in Dataflow Matrix Machines and Generalized Recurrent Neural Nets_, https://arxiv.org/abs/1606.09470

`modded-nanogpt` has already made a step in this direction by switching to _ReLU(x)*ReLU(x)_ activation function:

>         `x = F.relu(x).square() # https://arxiv.org/abs/2109.08668v2; ~1-2% better than GELU; suggested by @SKYLINEZ007 and @Grad62304977`
