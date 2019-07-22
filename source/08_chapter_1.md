# Introduction

## Background

Conventional automobile disk brakes are designed to decelerate vehicles by creating friction at the interface between the rotating disc and the braking pad. The geometries, forces and torques at play in this interface appear deceptively simple, yet the vibrations introduced into the system are not easily predicted or modeled whereas in practice oscillations are often observed, or rather heard, in the form of creep groan, squealing and similar. 

For decades [@Akay.2002] engineers have attempted to understand this particular Noise, Vibration and Harshness (NVH) phenomenon and attempted to determine predictive measures that would help determine under which conditions exactly these phenomena occur. With the growth of computational resources and thus growing simulation capabilities, complex numerical models based on several fundamental theories of friction [@N.M.Kinkaid.2003] have become feasible yet fail to capture the _key information_ required to develop a general-purpose model that would reflect the results obtained in experiments to a satisfying degree.

Recent developments in computational power, neural networks and optimization algorithms have lead to the practical application of large artificial neural networks (ANNs) to many problem domains. ANNs are based on connected neurons, which pass information through the network when activated. The key advantages of ANNs are their applicability to practically any datatype and their ability to learn complex nested features that make up the input data. This has been immensely successful in image recognition and generation. The results in time-series classification and generation have been equally impressive, driven largely by the field of speech recognition and processing.

The problem domain of time-series classification can be naturally split into shape- or feature-based or direct classification _(insert figure)_. In the case of the currently best-performing classifiers on the globally recognized UCR archive [@UCRArchive2018] are exclsuively ANNs that consume the time-series directly without going through manual/automatic preprocessing.

Existing NN architectures that perform well on time-series classification (excluding image-based time-series networks) are Multi-Layer-Perceptrons, Fully-Convolutional-Networks and Resnets [@Wang.11202016] as well as multi-scale CNNs [@Cui.3222016]. Karim et al. [@Karim.2018] have combined these architectures with attentive LSTM networks to circumvent the need for preprocessing for multilayered CNNs and gain the temporal nature of time-series data as information in long-short-term-memory.

Ensemble learning methods are learning algorithms that construct a set of weaker classifiers and then classify new samples by taking a (weighted) vote of the individual classifiers’ predictions. This is typically used to mitigate the high cost of training a strong classifier, be it due to dataset limitations or cost of computation. 

A recent development in neural network research is the attempt to bring ensemble learning approaches into the training and discovery of Neural Network based models [@Bagnall.2015]. The reasoning is that such an approach combines the best of two worlds: the ability to discover new neural architectures faster while learning a model for a specific application. In addition, providing more detailed insight into what features are being learned at individual layers or encoded in its tensors (higher-dimensional matrices) becomes possible.

One implementation of this that has received widespread attention is the AdaNet algorithm and its Tensorflow implementation under the same name [1,2]. To the knowledge of the author, Adanet estimators have not been built for this special case of time-series classification and characterization.

The objective of this thesis is to arrive at a neural architecture that performs better at classifying brake squealing than hitherto introduced models [@Karim.2018] and encodes information about the underlying system via algorithmic means.

To that end the state-of-the-art in time-series classification is examined and partly replicated by implementing and applying a recent innovation in neural architectures, the bi-directional LSTM network, to a benchmark time-series dataset [@UCRArchive2018] to compare against the result recounted in [@DanielSchoepflin.2019]. 

For the AdaNet algorithm to perform favorably, a number of special estimators and subnetwork types need to be defined. To this end, the AdaNet algorithm and published libraries are to be used. This requires the programming of tf.estimators and ada.subnetworks.

The selection of a resulting network structure to be benchmarked to evaluate the resulting network depends on Verifying the generalizability of the resulting network architecture is proposed to be conducted via cross-training between datasets from different brake systems [Schoepflin].

## The style of the citation is determined by the ref_format.csl file. For example, cite like this 

<!-- 
To include a reference, add the citation key shown in the references.bib file.
-->

## Maths

Numbered equations are assisted by installing [pandoc-crossref](https://github.com/lierdakil/pandoc-crossref):

$$ \rho c \frac{\partial T}{\partial t} =  \frac{\partial q} {\partial x} $$ {#eq:yourlabel}

Now you can reference your equations (@eq:yourlabel) inline. If using pandoc-crossref, add the following to each relevant section of the makefile. 

```--filter pandoc-crossref``` 

Non numbered equations:
$$ \rho c \frac{\partial T}{\partial t} =  \frac{\partial q} {\partial x} $$

## The middle bit

This is the middle bit. Phasellus quis ex in ipsum pellentesque lobortis tincidunt sed massa. Nullam euismod sem quis dictum condimentum. Suspendisse risus metus, elementum eu congue quis, viverra ac metus. Donec non lectus at lectus euismod laoreet pharetra semper dui. Donec sed eleifend erat, vel ultrices nibh. Nam scelerisque turpis ac nunc mollis, et rutrum nisl luctus.

Cras eleifend velit diam, eu viverra mi volutpat ut. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec finibus leo nec dui imperdiet, tincidunt ornare orci venenatis. Maecenas placerat efficitur est, eu blandit magna hendrerit eu.

### Subsection of the middle bit

This is a subsection of the middle bit. Quisque sit amet tempus arcu, ac suscipit ante. Cras massa elit, pellentesque eget nisl ut, malesuada rutrum risus. Nunc in venenatis mi. Curabitur sit amet suscipit eros, non tincidunt nibh. Phasellus lorem lectus, iaculis non luctus eget, tempus non risus. Suspendisse ut felis mi.

## Summary of chapters

<!-- 
For italic, add one * on either side of the text
For bold, add two * on either side of the text
For bold and italic, add _** on either side of the text
-->

This is a brief outline of what went into each chapter. **Chapter 1** gives a background on duis tempus justo quis arcu consectetur sollicitudin.  **Chapter 2** discusses morbi sollicitudin gravida tellus in maximus.  **Chapter 3** discusses vestibulum eleifend turpis id turpis sollicitudin aliquet.  **Chapter 4** shows how phasellus gravida non ex id aliquet. Proin faucibus nibh sit amet augue blandit varius.


