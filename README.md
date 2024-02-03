ForwardProblemX: A visual of the model's ability to predict the solution of a dynamical system from initial conditions and external forcing.
The examples shown are of model predictions from data on which the model was not trained. The agreement indicates the model has learned 
the dynamical system's dynamics and generalizes well to new, unseen data. 

FourierBasisCoeffChainX: A visual of the sampler chain and marginal densities of the parameters of the external forcing function's 
basis coefficients. This is used to generate function posterior plots. 

FunctionPosteriorX: A visual of the posterior distribution over external torque functions using traces/samples from the markov chain.

ModelPosteriorX: These functional posterior traces were fed back into the ODE solver and the neural operator to showcase how sensitive
the model is to the uncertainty in the inferred torque function distribution. This was also done to compare the solution distribution
between the ODE Solver and DeepONet models. The tight overlap indicates agreement between how the ODE solver and DeepONet warp the 
distribution over external forcings to the distribution over solutions. 

The subscript _u1u2 indicates both angular position and frequency used for inference, _u1 uses position only, _u2 velocity only. 
