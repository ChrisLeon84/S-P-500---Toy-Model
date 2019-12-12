# S-P-500---Toy-Model
Toy model, based on Geometric Brownian model (see https://en.wikipedia.org/wiki/Geometric_Brownian_motion). 

Two important variables correspond to rate of return and voltaility (&mu; and &sigma;<sup>2</sup>). First, guessed them by qualitatively matching with S&P500. Interestingly, later I looked in the literautre and others got empirical numbers from end-of-week historic data and it matched quite closely to my crude method.

Putting these numbers in and generated a simulation for a 10 year period. I then tried to see if you can use parameter estimation from the first 5 years to predict the next 5 years. This was done using,

E[S<sub>t</sub>] = S<sub>0</sub> exp [&mu; t] 


The curve was in the 'cone of uncertainty' sometimes, but the cone could be really wide. 

This was just a toy model, however elements may be incorparated later for soemthing more sophisticated.
