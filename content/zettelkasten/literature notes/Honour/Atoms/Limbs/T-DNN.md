To add: 
The training part of DNNs are usually considered opaque because we are ... -> find the source. 

===Training DNN Thing===
However, some might argue that because a DNN is liable to fitting on the wrong function, it is fundamentally unreliable. 

For example, if we consider a compass produced and utilised within a scientific experiment. We are hoping that it picks up on the earths magnetic fields, however other strong magnetic forces may interfere. The compass is doing what is was produced for - picking up on a magnetic field. Similar to a DNN which picks up on a certain function based on patterned features within the input data. It is impossible to control that it will pick up on the correct function every-time because the context of what the "correct" function is will change. Similar to if a researcher wants to use a compass to measure the magnetic field of an object in another room, instead of the earth's. 

Therefore, for the reliability of the training stage of the DNN we need to defer to the contexts of its experimental use. What we are interested in is producing an algorithm which is trying to pick up on what the researchers want it to pick up on. Similar to any other *causal* scientific instrument which is constructed to take advantage of a certain phenomena. DNNs must be constructed with this phenomena in mind. Examples of this type of interference would be picking diverse training data . [[Method Learning - Pragmatic Approach to Deep Learning]], Ortmann, [[The Epistemology of AI-driven Science The Case of AlphaFold]]

Robustness Part

While robustness has long been a part of ML research, some have still argued that we need access to the internal rules that a model makes while training. We argue that this is unnecessary and stems from confusion to what the training-process of a DNN actually is. 

Why doesn't the justification of training lead to the justification of the model? Because models are justified in very different ways. 