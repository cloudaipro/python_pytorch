https://primo.ai/index.php?title=Activation_Functions
![Neural Network Activation Functions: a small subset!](https://aman.ai/primers/ai/assets/activation/1.png)

By definition, activation functions
- Are nonlinear. Repeated applications of (w*x+b) without an activation function results in a function of the same (affine linear) form. The nonlinearity allows the overall network to approximate more complex functions.
- Are differentiable, so that gradients can be computed through them. Point dis- continuities, as we can see in Hardtanh or ReLU, are fine.

The following are true for the functions:
- They have at least one sensitive range, where nontrivial changes to the input result in a corresponding nontrivial change to the output. This is needed for training.
- Many of them have an insensitive (or saturated) range, where changes to the input result in little or no change to the output.
