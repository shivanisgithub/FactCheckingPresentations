# Explaining Deep Learning models for Fact-Checking 
## How do different explanation presentation strategies of feature and data attribution techniques affect non-expert understanding?
*Shivani Singh*

This repository contains the codebase for a Thesis Submitted to EEMCS Faculty Delft University of Technology, in Partial Fulfilment of the Requirements for the Bachelor of Computer Science and Engineering

### Structure

This repository contains three Jupyter Notebooks. Each of these contain the codebase for presenting the explanation methods as shown in this [Figma template](https://www.figma.com/community/file/1194688306111467424). Of course you are welcome to use this code for other purposes than creating [Figma Prototypes](https://www.figma.com/proto/PIntG4MgCfXVTJ3N0hEnIQ/BEP_shivi?node-id=79%3A2429&starting-point-node-id=79%3A2429).

#### Requirements

- FEVER. All three explanation methods are computed and presented on test data of the [FEVER dataset](http://www.eraserbenchmark.com/zipped/fever.tar.gz)

- ExPred. If you wish to run the juypter notebook on ExPred presentations, you require [ExPred: the Deep Neural model](https://github.com/JoshuaGhost/expred), which is an implementation of the paper [Explain and Predict, and then Predict Again](https://dl.acm.org/doi/abs/10.1145/3437963.3441758). Our juypter notebook builds on top of the Showcase for ExPred. Before using the notebook we suggest you clone ExPred and follow their instructions on setting it up.

- LIME.  In order to run the juypter notebook on Feature attribution presentations, you require results from [LIME](https://github.com/marcotcr/lime), which is an implementation of the paper ["Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938). In the juypter notebook the required input is explained. Before using the notebook you need normalised results of running LIME on a claim. As long as the input format is the same, other feature attribution methods such as SHAP or Integreated gradients should work as well. We used the [Captum library for LIME](https://captum.ai/api/lime.html) and the implementation of (instert link to Annabel's implementation).

- Instance attribution. In the notebook you can find an example of the kind of input data you need. In our case the data was retreived from [this implementation](https://github.com/HatchIing/InstanceAttribution). You can use your own implementation of k-nn of course, as long as the format of the input is the same.

- Python 3.8. The notebooks have been used with this versions. There is no guarentee there will be no issues when other versions are used.


### Reproducing the Research

Here are the steps for those who are interested in reproducing the research.

1. Clone this repository
2. Run the provided Jupyter Notebooks
3. Paste the results in the Figma Templates
