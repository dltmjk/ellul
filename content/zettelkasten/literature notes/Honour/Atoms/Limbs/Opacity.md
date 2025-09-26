General Plan 

Instruments: 
A microscope doesn't provide an explanation of its results. It's results are only valid in the context of, for example, a Newtownian theory. DNNs, like most scientific instruments which pick up on causal relationships with the world, also do not provide explanations. However, the key difference is that most scientific instruments are specifically constructed in the process of an experiment, therefore their explanatory role is already fulfilled. 

DNNs do not have their luxury, as a general statistical tool, their prevalence has led to misconceptions in which they have to account for the results in a way that most other instruments are not expected to. If we view a DNN as a model, the same rules apply. Scientific models are constructed in view of a specific theory. 

(how to expand?)



To Write: The advantage that treating DNNs as scientific instruments gives us. We treat the DNN as one part of the scientific process. We only have problems with opaqueness when we treat a DNN as standing in for all parts of the scientific process. However, 

1. Note down each reason for opacity 
2. Reasons for opacity 
	1. Evaluate as a scientific instrument 

We should only care about reliability, if the DNN is a scientific instrument. Can reliability ever be secured? 

Arguments for Opacity. 

There is a property $\chi$ that when applied to a scientific model makes it opaque. The lack, or toning down, of this property increases the *transparency* of a system. If more than two $\chi$ properties are present, the lowering of one doesn't change the opaqueness of a system. If a system is opaque because of its dimensionality, modifying the size will not make a difference to the overall opaqueness. In attempting to find which properties actually guarantee opaqueness, we can look at examples of inherently transparent statistical algorithms, of which both decision trees and naive bayes classifiers are examples. 

Rundown of both 

In what qualities does a DNN differ from these two algorithms? 

Zerelli “Tractability/Intelligibility/Fathomability Distinction” 

Categories for Opaqueness 
Fathomability 
Intelligibility 
Tractability 

Zerilli argues for model opacity along the lines of *linearity* and *dimensionality*. A linear system with fewer dimensions is more *fathomable* than an alternate higher dimensional system. In which *fathomability* concerns a human observer who, in the former low-dimensional case, is able to "contemplate the entire model at once" (Lipton 2017, 4) (Zerelli, 7). Therefore, dimensionality and fathomability are inversely correlated. An unfathomable system, for example, would be an extremely large computer simulation model with billions of parts. However, as long as this simulation maintains linearity, it retains another two of  Zerelli's properties - intelligibility and tractability. Tractability is whether a model can be run on a machine whereas intelligibility is if the relationship between a models subparts can be determined despite size. 

Zerelli's speaks of opacity in respect to these properties. For example, a computer program which multiplies large numbers may be opaque due to its un-*fathomability* given that a human agent cannot possibly hope to work through each binary operation the program performs. However, it still maintains the properties of tractability and intelligibility.

![[Pasted image 20250926104216.png]]

Burrell (2016): “[DNNs] are opaque in the sense that if one is a recipient of the output of the algorithm (the classification decision), rarely does one have any concrete sense of how or why a particular classification has been arrived at from inputs.

Creel 
Creel extends these concepts of opacity and transparency by providing three ways in which an algorithm can be opaque. 


Sogaard
The common arguments for DNN opacity refer to the status of either model size, continuity, nonlinearity, instrumentality, or incrementality (Sogaard). Due to the nature of DNN construction, as a instrument heavily reliant on orderings of training data, Skogaard claims that DNNs are opaque in regards to both training and prediction. Naming these two types of opacity training and inference opacity respectively. 

Boge makes a similar distinction between h(ow)-opacity, which concerns how a DNN alters its function in response to training data, and w(hat)-opacity which concerns what function was learned in the course of training. 

However, is this really opaqueness? 





(What are the different ways DNNs can be opaque?) Opaque in regards to how it arrived to a prediction and the lack of explanation along with the prediction. 
