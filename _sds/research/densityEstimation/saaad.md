---
layout: single
title: Potential Research - Project SAAAD
permalink: /sds/research/densityEstimation/saaad/
author_profile: true
header:
  overlay_color: "#5e616c"
  overlay_image: /sds/research/densityEstimation/sahde/notes/MDE_20161010_141708_01.jpg
  caption: 
excerpt: 'for Scalable Mathematical Statistical Experiments.<br /><br /><br />'
---

{% include toc %}

# Project SAAAD:<br /> Scalable Adaptive Auto-encoded Anomaly Detection

Project SAAD is an effort to evaluate the possibilites for further extensions of [Project SAHDE](https://lamastex.github.io/scalable-data-science/sds/research/densityEstimation/sahde/) via *auto-encoder mapped regular pavings* as *auto-encoded statistical regular pavings* that are ultimately capable of appropriate tree arithmetics formalised and explored in *Relevant Codes and Papers* section below.

This programme is partly supported by:

* [databricks academic partners program](https://academics.cloud.databricks.com) for distributed cloud computing
* research time for this project was party due to:
	* 2015, 2016 by the project [CORCON: Correctness by Construction](http://corcon.net/about/), Seventh Framework Programme of the European Union, Marie Curie Actions-People, International Research Staff Exchange Scheme with counter-part funding by The Royal Society of New Zealand 
	* 2017, Researcher Position, Department of Mathematics, Uppsala University, Uppsala, Sweden. 

## Relevant Codes and Papers

<ul>
<li>Data-adaptive histograms through statistical regular pavings, Raazesh Sainudiin, Gloria Teng, Jennifer Harlow and Warwick Tucker, 2016 (<a class="linkitem" href="http://lamastex.org/preprints/20161121optMAPMDE.pdf">PDF</a> 1.8MB)</li>

<li>MRS 2.0: A C++ Class Library for Statistical Set Processing and Computer-Aided Proofs in Statistics (Version 2.0) [Software], Jennifer Harlow, Raazesh Sainudiin, Gloria Teng, Warwick Tucker and Thomas York, Available from <a class="linkitem" href="https://github.com/lamastex/mrs2">https://github.com/lamastex/mrs2</a>, 2017</li>

<li>An auto-validating, trans-dimensional, universal rejection sampler for locally Lipschitz arithmetical expressions, Raazesh Sainudiin and Thomas York, <a class="linkitem" href="http://interval.louisiana.edu/reliable-computing-journal/volume-18/reliable-computing-18-pp-015-054.pdf">Reliable Computing, vol.18, pp.15-54</a>, 2013 (<a class="linkitem" href="http://lamastex.org/preprints/avs_rc_2013.pdf">PDF</a> 2612KB)</li>

<li>Posterior expectation of regularly paved random histograms, Raazesh Sainudiin, Gloria Teng, Jennifer Harlow and Dominic Lee, <a class="linkitem" href="http://dx.doi.org/10.1145/2414416.2414422">ACM Trans. Model. Comput. Simul. 23, 1, Article 6, 20 pages</a>, 2013 (<a class="linkitem" href="http://lamastex.org/preprints/SubPavingMCMC.pdf">PDF</a> 1864KB)</li>

<li>Mapped Regular Pavings, Jennifer Harlow, Raazesh Sainudiin and Warwick Tucker, <a class="linkitem" href="http://interval.louisiana.edu/reliable-computing-journal/volume-16/reliable-computing-16-pp-252-282.pdf">Reliable Computing, vol. 16, pp. 252-282</a>, 2012 (<a class="linkitem" href="http://lamastex.org/preprints/MappedRegularPaving.pdf">PDF</a> 972KB)</li>

<li>Statistical regular pavings to analyze massive data of aircraft trajectories, Gloria Teng, Kenneth Kuhn and Raazesh Sainudiin, <a class="linkitem" href="http://arc.aiaa.org/doi/abs/10.2514/1.I010015">Journal of Aerospace Computing, Information, and Communication, Vol. 9, No. 1, pp. 14-25</a>, doi: 10.2514/1.I010015, 2012 (<a class="linkitem" href="http://lamastex.org/preprints/AAIASubPavingATC.ps">PS</a> 31MB or lossy <a class="linkitem" href="http://lamastex.org/preprints/AAIASubPavingATC.pdf">PDF</a> 2.9MB or <a class="linkitem" href="http://lamastex.org/preprints/AAIASubPavingATC_PNG.zip">zipped 26 PNG pages</a>) </li>
</ul>

# Anomaly Detection with Autoencoders

## References
* Some quick mathematical, statistical, computational background readings:
  * [Anomaly detection - Wikipedia](https://en.wikipedia.org/wiki/Anomaly_detection)
  * [Auto Encoders Chapter - Deep Learning Book](http://www.deeplearningbook.org/contents/autoencoders.html) (see references therein)
  * [Autoencoders - Stanford Tutorial](http://ufldl.stanford.edu/tutorial/unsupervised/Autoencoders/)
  * [Digit recognition (Image Search)](http://elkews.com/preview/565650)
  * ...
* Computing frameworks for scalable deep learning and auto-encoders in particular
  * [H2O Deep learning](http://h2o2016.wpengine.com/wp-content/themes/h2o2016/images/resources/DeepLearningBooklet.pdf)
  * Sparkling Water - H2O with Spark
  * IBM's BigDL in Spark
  * TensorFlow and Spark TensorFrames

 
# Some Background on Existing Industrial Solutions

* Some interesting industrial solutions already exist, including:
  * [https://community.tibco.com/wiki/anomaly-detection-autoencoder-machine-learning-template-tibco-spotfirer](https://community.tibco.com/wiki/anomaly-detection-autoencoder-machine-learning-template-tibco-spotfirer)
  * and others...

The content in the next section is just a 
```%sh
$ wget -k https://community.tibco.com/wiki/anomaly-detection-autoencoder-machine-learning-template-tibco-spotfirer
$ pandoc -f html -t markdown anomaly-detection-autoencoder-machine-learning-template-tibco-spotfirer > ex.md
$ vim ex.md
$ !date
$ Fri Aug 18 18:33:05 CEST 2017
```
It is meant to give a reasonably standard industrial solution to the problem and help set the context for industrially beneficial research directions. There are other competing solutions, but we will focus on this example for concreteness.

---
---

## Anomaly Detection with Autoencoder Machine Learning - Template for TIBCO Spotfire®

By Venkata Jagannath from [https://community.tibco.com/users/venkata-jagannath](https://community.tibco.com/users/venkata-jagannath)

Anomaly detection is a way of detecting abnormal behavior. The technique
first uses machine learning models to specify expected behavior and then
monitors new data to match and highlight unexpected behavior.


Use cases for Anomaly detection
-------------------------------

**Fighting Financial Crime** – In the financial world, trillions of
dollars’ worth of transactions happen every minute. Identifying
suspicious ones in real time can provide organizations the necessary
competitive edge in the market. Over the last few years, leading
financial companies have increasingly adopted big data analytics to
identify abnormal transactions, clients, suppliers, or other players.
Machine Learning models are used extensively to make predictions that
are more accurate.

**Monitoring Equipment Sensors** – Many different types of equipment,
vehicles and machines now have sensors.  Monitoring these sensor outputs
can be crucial to detecting and preventing breakdowns and disruptions.
 Unsupervised learning algorithms like Auto encoders are widely used to
detect anomalous data patterns that may predict impending problems. 

**Healthcare claims fraud** – Insurance fraud is a common occurrence in
the healthcare industry. It is vital for insurance companies to identify
claims that are fraudulent and ensure that no payout is made for those
claims. The economist recently published an article that estimated \$98
Billion as the cost of insurance fraud and expenses involved in fighting
it. This amount would account for around 10% of annual Medicare &
Medicaid spending. In the past few years, many companies have invested
heavily in big data analytics to build supervised, unsupervised and
semi-supervised models to predict insurance fraud.

**Manufacturing detects** – Auto encoders are also used in manufacturing
for finding defects. Manual inspection to find anomalies is a laborious
& offline process and building machine-learning models for each part of
the system is difficult. Therefore, some companies implemented an auto
encoder based process where sensor equipment data on manufactured
components is continuously fed into a database and any defects (i.e.
anomalies) are detected using the auto encoder model that scores the new
data.
[Example](http://webserv.lurpa.ens-cachan.fr/dcds_series/dcds11/fileadmin/user_upload/pdf/tilbury-dcds2011.pdf)

Techniques for Anomaly detection
--------------------------------

Companies around the world have used many different techniques to fight
fraud in their markets. While the below list is not comprehensive, three
anomaly detection techniques have been popular -

**Visual Discovery** - Anomaly detection can also be accomplished
through visual discovery. In this process, a team of data
analysts/business analysts etc. builds bar charts; scatter plots etc. to
find unexpected behavior in their business. This technique often
requires prior business knowledge in the industry of operation and a lot
of creative thinking to use the right visualizations to find the
answers.

**Supervised Learning** - Supervised Learning is an improvement over
visual discovery. In this technique, persons with business knowledge in
the particular industry label a set of data points as normal or anomaly.
An analyst then uses this labelled data to build machine learning models
that will be able to predict anomalies on unlabeled new data.

**Unsupervised Learning** - Another technique that is very effective but
is not as popular is Unsupervised learning. In this technique, unlabeled
data is used to build unsupervised machine learning models.  These
models are then used to predict new data. Since the model is tailored to
fit normal data, the small number of data points that are anomalies
stand out.

Some examples of unsupervised learning algorithms are -

**Auto encoders** – Unsupervised neural networks or auto encoders are
used to replicate the input dataset by restricting the number of hidden
layers in a neural network. A reconstruction error is generated upon
prediction. Higher the reconstruction error, higher the possibility of
that data point being an anomaly.

**Clustering** – In this technique, the analyst attempts to classify
each data point into one of many pre-defined clusters by minimizing the
within cluster variance. Models such as K-means clustering, K-nearest
neighbors etc. used for this purpose. A K-means or a KNN model serves
the purpose effectively since they assign a separate cluster for all
those data points that do not look similar to normal data.

**One-class support vector machine** – In a support vector machine, the
effort is to find a hyperplane that best divides a set of labelled data
into two classes. For this purpose, the distance between the two nearest
data points that lie on either side of the hyperplane is maximized. For
anomaly detection, a One-class support vector machine is used and those
data points that lie much farther away than the rest of the data are
considered anomalies.

**Time Series techniques** – Anomalies can also be detected through time
series analytics by building models that capture trend, seasonality and
levels in time series data. These models are then used along with new
data to find anomalies. [Industry example](http://nerds.airbnb.com/anomaly-detection/)

Auto encoders explained
-----------------------

Autoencoders use unsupervised neural networks that are both similar to
and different from a traditional feed forward neural network. It is
similar in that it uses the same principles (i.e. Backpropagation) to
build a model. It is different in that, it does not use a labelled
dataset containing a target variable for building the model. An
unsupervised neural network also known as an Auto encoder uses the
training dataset and attempts to replicate the output dataset by
restricting the hidden layers/nodes.

![](https://d2wh20haedxe3f.cloudfront.net/sites/default/files/autoencode_doc1.png)

The focus on this model is to learn an identity function or an
approximation of it that would allow it to predict an output that is
similar the input. The identity function achieves this by placing
restrictions on the number of hidden units in the data. For example, if
we have 10 columns in a dataset and only five hidden units, the neural
network is forced to learn a more restricted representation of the
input. By limiting the hidden units, we can force the model to learn a
pattern in the data if there indeed exists one.

Not restricting the number of hidden units and instead specifying a
‘sparsity’ constraint on the neural network can also find an interesting
structure.

Each of the hidden units can be either active or inactive and an
activation function such as ‘tanh’ or ‘Rectifier’ can be applied to the
input at these hidden units to change their state.

![](https://d2wh20haedxe3f.cloudfront.net/sites/default/files/autoencode_doc2.png)

Some forms of auto encoders are as follows –

-   Under complete Auto encoders
-   Regularized Auto encoders
-   Representational Power, Layer Size and Depth
-   Stochastic Encoders and Decoders
-   Denoising Auto encoders

A detailed explanation of each of these types of auto encoders is
available
[here](http://www.deeplearningbook.org/contents/autoencoders.html).

Spotfire Template for Anomaly detection
---------------------------------------

TIBCO Spotfire’s Anomaly detection template uses an auto encoder trained
in H2O for best in the market training performance. It can be configured
with document properties on Spotfire pages and used as a point and click
functionality.

[Download the
template](https://community.tibco.com/modules/anomaly-detection-template-tibco-spotfirer)
from the Component Exchange.  See documentation in the download
distribution for details on how to use this template

---
---

# Questions for AIM Day

## Q.1 Semi-supervised Anomaly Detection with Human-in-the-Loop

![](https://tr3.cbsistatic.com/hub/i/r/2016/04/15/c326870e-5682-40f6-9085-6e95cea67e7e/resize/770x/166a5883e09792f95d22f3382b8c581b/ai2-visual-credit-mit-csail.jpg)

### Introduction
Anomaly detection is a a subset of data mining where the task is to detect observations deviating from the expected pattern of the data. Important applications of this include fraud detection, where the task is to detect criminal or fraudulent acticity for example in for example credit card transactions or insurance claims. Another important application is in predictive maintenance where recognising anomalous observation could help predict the need for maintenance before the actual failure of the equipment.

The basic idea of anomaly detection is to establish a model for what is normal data and then flag data as anomalous if it deviates to much from the model. The biggest challenge for an anomaly detection algorithm is to discriminate between anomalies and natural outliers, that is to tell the difference between uncommon and unnatural data and uncommon but natural data. This distinction is very dependent of the application at hand, and it is very unlikely that there is one single classification aslgorithm that is to make this distinction in all applications. However, it it is often the case that a human expert is able to tell this difference, and it would be of great value to develop methods to feed this information back to the algorithm in an interactive loop. This idea is sometimes called active learning.

* What algorithms are there for incorporating active learning to anomaly detection? How can these be imnproved?
* Can one develop active learning anomaly detection based on autoencoders?
* How do you avoid overfitting to known types of anomalies?

### Q.1.1 Interactive Visualisation of the Autoencoder's Layers

Given the crucial requirement for rich visual interactions between the algorithm and the human-in-the-loop, what are natural open-source frameworks for programmatically enriching this human-algorithm interaction via visual inspection and interrogation (such as SVDs of activations of rare anomalous events for instance).

* http://projector.tensorflow.org

### Q.1.2 Parametric families of *HiL-Loss*

Is there a natural mathematical statistical argument for parametric families of loss functions for tuning hyper-parameters, where the loss functions can account for the budgeting costs for a set of human beings with different hourly wages  who are capable of tagging different types of events with distinct rare probabilities within a generic human-in-the-loop model for anomaly detection?

For example, such a loss could be justified using notions such as query-efficiency in the sense of involving only a small amount of interaction with the teacher/domain-expert ([Supervised Clustering, NIPS Proceedings, 2010](https://papers.nips.cc/paper/4115-supervised-clustering.pdf). Ideally, this loss can be extended to auto-encoder networks with an additional node(s) for classifying rare anomalous events of several known types via interaction with the domain expert.    

## Background Information

### NEWS:
* [MIT shows how AI cybersecurity excels by keeping humans in the loop](http://www.techrepublic.com/article/mit-shows-how-ai-cybersecurity-excels-by-keeping-humans-in-the-loop/)

### RESEARCH
* [AI2: Training a big data machine to defend, Kalyan Veeramachaneni, Ignaciao Arnaldo, Alfredo Cuesta-Infante, Vamsi Korrapati, Costas Bassias and Ke Li, 2016](http://people.csail.mit.edu/kalyan/AI2_Paper.pdf)
* [Supervised Clustering, Pranjal Awasthi and Reza Bosagh Zadeh, NIPS Proceedings, 2010](https://papers.nips.cc/paper/4115-supervised-clustering.pdf)
  * [Video Lecture 4 minutes](http://www.quizover.com/oer/course/supervised-clustering-by-reza-bosagh-zadeh-videolectures-net-oer)

## Relevant Papers

* ["Adversarial Autoencoders" Ian J. Goodfellow et al.](https://arxiv.org/pdf/1511.05644.pdf)
* ["Variational Autoencoder based Anomaly Detection using Reconstruction Probability", Jinwon An and Sungzoon Cho](http://dm.snu.ac.kr/static/docs/TR/SNUDM-TR-2015-03.pdf)
* ["Incorporating Expert Feedback into Active Anomaly Discovery", Das et al.](http://web.engr.oregonstate.edu/~tgd/publications/das-wong-dietterich-fern-emmott-incorporating-expert-feedback-into-active-anomaly-discovery-icdm2016.pdf)
* ["Loda: Lightweight on-line detector of anomalies", Tomáš Pevný](https://link.springer.com/content/pdf/10.1007%2Fs10994-015-5521-0.pdf)


## Codes

Some interesting random codes that need exploring and experimenting:

* [https://github.com/jramapuram/LSTM_Anomaly_Detector](https://github.com/jramapuram/LSTM_Anomaly_Detector)
* ...

## LICENSE

Copyright 2016, 2017 Raazesh Sainudiin

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



## Whiteboard discussion notes on 2017-08-18.
 
We will eventually lua/la/ka-tex mathematically from here...

![auto-encoder mapped regular pavings and naive probing](notes/saaad0.jpg)

## Random thoughts regarding anomaly detection with emphasis on fraud detection

Normally, anomaly detection is treated as an **unsupervised learning problem**, where the machine tries to build a model of the training data. Since an anomaly per definition is a data point that in some way is uncommon, it will not fit the machine's model, and the model can flag it as an anomaly. In the case of fraud detection, it is often the case that a small fraction (perhaps 1 ppm) of the data points represent known cases of fraud attempts. It would be wasteful to throw away this information when building the model. This would mean that we no longer have a unsupervised learning problem, but a **semi-supervised learning problem**. In a typical semi-supervised learning problem, the problem is to assign predefined labels to datapoints when the correct label is only known for a small fraction of the dataset. This is a very interesting idea, since it allows for using the power of big data, without having to pay the cost of correctly labeling the whole dataset. If we translate our fraud detection problem to this setting it means that we hava a big collection of datapoints which we want to label as either "fraud" or "non-fraud". However, in contrary to the standard setup for semi-supervised learning, we only have known examples from the "fraud" class. This (at least formally) puts us in another class of learning problems, namely **PU learning**, where the dateset is split into two classes, the positive class, *P*, and the unlabel class, *U*.

After running the fraud detection model on our data, we are likely to be given suspected cases of fraud, which can be correctly labelled by an expert. This means that we can improve our dataset with more labelled points and retrain our model using the new information. At this point however, we probably have some confirmed examples of the non-fraud class, and from this point we no longer have a PU learning problem.

One important note about running a semi-supervised learning for anomaly detection is that some people actually advise against training a model on known anomalies, since this will produce a model that is good at detecting anomalies of known kinds, but which probabliy is less able to detect new kind of anomalies. This is extra important in fraud detection, since fraudsters are likely to continually come up with new schemes to trick the model.

Another related thought is that with the relabelling scheme described above, all datapoints labelled non-fraud will be such points which the model originally had problems distiguishing from fraud. This is likely to introduce instability to the model.   For this reason, it might be worthwile to put some effort into correctly classifying also some datapointcalls ts which are very unlikely to be fradulent. With respect to this, it might be interesting to read some of the literature on **active learning**. Active learning is an iterative type of semi-supervised learning where the learning algorithm is active and can purposefully queary a user for correct data labels. Ideally, the algorithm can determine which unlabelled points it would be most befefitial to learn the correct labels for.

## Interesting deep learning algorithms
* *Autoencoders*

  Neural networks that are trained to reproduce the indata. Come in different flavours both with respect to depth and width, but also with respect to how overlearning is prevented. Can be used to detect anomalies as those datapoints that are poorly reconstructed by the network. Can also be used for dimennsion reduction in a data preprocession step. Subsequently other anomaly detection techniques can be applioed to the transformed data.
    * ["Autoencoders, Unsupervised Learning, and Deep Architectures", Pierre Baldi.](http://proceedings.mlr.press/v27/baldi12a/baldi12a.pdf)
* *Variational autoencoders*

    Variational autoencoders are a varaiant of autoencoders (or is it the other way around?) where the network is trying to transform the data to a pior distribution (usually multivariate normal). That is, the lower dimensional representation of the data that you get from standard autoencoder will be distributed according to the prior distribution in the case of a variational autoencoder. This means that you can feed data from the prior distribution backwards through the network to generate new data from a distribution close to the one of the original, authentic data. Of course you can also use the network to detect outliers in the dataset by comparing the transformed dataset with the prior distribution.
    * ["Variational Autoencoders Explained", Kevin Frans](http://kvfrans.com/variational-autoencoders-explained/)
    * ["Variational Autoencoder based Anomaly Detection using Reconstruction Probability", Jinwon An and Sungzoon Cho](http://dm.snu.ac.kr/static/docs/TR/SNUDM-TR-2015-03.pdf)
    * ["Tutorial on Variational Autoencoders", Carl Doersch](https://arxiv.org/abs/1606.05908)
* *Adversional autoencoders*

     Adversarial autoencoders  have some conceptual similarities with variational autoencoders in that they also are capable of generating new (approximate) samples of the dataset. In fact, from my superficial comparison of the two types of autoencoders, it seems like the biggest difference between them is not so much how they model the network, but how they are trained. Adersional autoencoders are based on the idea of GANs (Generative adversarial networks). This is how I understand the workings of a GAN. Two neural networks are randomly initialized and random indata from a specified distribution is fed into the first network (the generator). Then the outdata of the first network is fed as indata to the other network (the disciminator). Now the job for the discriminator is to correctly discriminate forged data coming from the generator network from authentic data. The job for the generator network is to as often as possible fool the discriminator. This can be interpreted as a zero-sum game in the sense of game theory, and training a GAN is then seen to be equivalent to finding the Nash-equilibrium of this game. Fidning such a equibrilium is of course far from trivial but it seems like good results can be achieved by training the networks iteratively side by side through backpropagation. I don't think this is really relevant for us, but I think it is a bit interesting on a meta level that this generator/discriminator rivalry is a bit reminiscent of the relationshop between the fraudster and the anomaly detector.
     * ["Generative Adversarial Nets" Ian J. Goodfellow et al.](https://arxiv.org/pdf/1406.2661.pdf)
     * ["Adversarial Autoencoders" Ian J. Goodfellow et al.](https://arxiv.org/pdf/1511.05644.pdf)
     * ["Generative Adversarial Networks Explained", Kevin Frans](http://kvfrans.com/generative-adversial-networks-explained/)
* *Ladder networks*

    Ladder networks is a class of networks specially developed for semi-supervised learning. It aims at combining supervised and unsupervised learning at every level of the network. The method has made very impressive results on classifying the MNIST dataset, but it is still open how well it performs on other datasets.
    * ["Introduction to Semi-Supervised Learning with Ladder Networks", Rinu Boney](http://rinuboney.github.io/2016/01/19/ladder-network.html)
    * ["Semi-Supervised Learning with Ladder Networks", Antti Rasmus et al.](https://arxiv.org/pdf/1507.02672.pdf)

## Active Anomaly Discovery
*Active Anomaly Discovery* (AAD) is a method for incorporating expert feedback to the learning algorithm. The basic idea is that the loss function is calculated based on how many non-interesting anomalies it presents to the expert instead of the usual loss functions, like the reconstruction error. The original impementation of AAD is based on an anomaly detector called *Loda* (Lightweight on-lin detector of anomalies), but it has also been impelemnted on other ensemble methods, like tree-based methods.

The Loda method might be extra interesting for us, and it might be worthwhile for us to take an extra look on it. The idea is to project the data to a random one-dimensional subspace, form a histogram and predict the log probability of an observed data point. Of course this is a very poor anomaly detector, but by taking the mean of large number of these weak anomaly detectors, we end up with a good anomaly detector. Remembering our previous discussions on t-digest and adaptive histogram density estimation, there might be something for us to add to this method.

* ["Loda: Lightweight on-line detector of anomalies", Tomáš Pevný](https://link.springer.com/content/pdf/10.1007%2Fs10994-015-5521-0.pdf)

* ["Incorporating Expert Feedback into Active Anomaly Discovery", Das et al.](http://web.engr.oregonstate.edu/~tgd/publications/das-wong-dietterich-fern-emmott-incorporating-expert-feedback-into-active-anomaly-discovery-icdm2016.pdf)

* ["Incorporating Feedback into Tree-based Anomaly Detection", Das et al.](http://poloclub.gatech.edu/idea2017/papers/p25-das.pdf)

## Visualisation
We should take a look at the following:
* http://projector.tensorflow.org