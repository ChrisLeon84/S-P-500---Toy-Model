# S-P-500---Toy-Model
Toy model, based on Geometric Brownian motion (see [here](https://en.wikipedia.org/wiki/Geometric_Brownian_motion) for more details). 

### Description

The value at some point in time, S<sub>t</sub>, is given by:

#### S<sub>t</sub> = S<sub>0</sub> exp [ (&mu;- &sigma;<sup>2</sup>/2)t + &sigma;W<sub>t</sub>]

where W<sub>t</sub> is a Wiener process (basically, a continuous random walk). The two parameters here correspond basically to rate of return and voltaility (&mu; and &sigma;<sup>2</sup>). First, I guessed them by qualitatively matching with S&P500. Interestingly, later I looked in the literautre and others got empirical numbers from end-of-week historic data and it matched quite closely to what I got.

Putting in these parameters I then generated a simulation for a 10 year period. I tried to see if you can use parameter estimation from the first 5 years to predict the next 5 years. Later did the same thing with a 20 year period. This was done using,

#### E[S<sub>t</sub>] = S<sub>0</sub> exp [&mu;t] 

#### Var[S<sub>t</sub>] = S<sub>0</sub><sup>2</sup> exp [2&mu;t] (exp [&sigma;<sup>2</sup>t]-1 )

The curve was in the 'cone of uncertainty' sometimes, but the cone could be really wide. 

This was just a crude toy model, however elements may be incorparated later for soemthing more sophisticated.
