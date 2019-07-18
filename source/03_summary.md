# Introduction {.unnumbered}

<!-- This is the abstract -->

Conventional automobile disk brakes are designed to decelerate vehicles by creating friction at the interface between the rotating disc and the braking pad. The geometries, forces and torques at play in this interface appear deceptively simple, yet the vibrations introduced into the system are not easily predicted or modeled whereas in practice oscillations are often observed, or rather heard, in the form of creep groan, squealing and similar. 

For decades [@Akay.2002] engineers have attempted to understand this particular Noise, Vibration and Harshness (NVH) phenomenon and attempted to determine predictive measures that would help determine under which conditions exactly these phenomena occur. With the growth of computational resources and thus growing simulation capabilities, complex numerical models based on several fundamental theories of friction [@N.M.Kinkaid.2003] have become feasible yet fail to capture the _key information_ required to develop a general-purpose model that would reflect the results obtained in experiments to a satisfying degree.

Recent developments in computational power, neural networks and optimization algorithms have lead to the practical application of large artificial neural networks (ANNs) to many problem domains. The problem domain of time-series 
The objective of this thesis is to arrive at a neural architecture that performs better at classifying brake squealing than hitherto introduced models and encodes information about the underlying system via algorithmic means.
To that end the state-of-the-art in time-series classification is examined and partly replicated by implementing and applying a recent innovation in neural architectures, the bi-directional LSTM network, to a benchmark time-series dataset to compare against the result recounted in [@Schoepflin]. 

~~For the AdaNet algorithm to perform favorably, a number of special estimators and subnetwork types need to be defined. To this end, the AdaNet algorithm and published libraries are to be used. This requires the programming of tf.estimators and ada.subnetworks~~


\pagenumbering{roman}
\setcounter{page}{1}
