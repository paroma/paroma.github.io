---
layout: default
title: Paroma Varma
---

## <a name="home"></a> Paroma Varma

### Ph. D. Student - Electrical Engineering - Stanford University  

### paroma [at] stanford [dot] edu - @paroma_varma

<img src="profile.jpg" align="middle"/>

I am a fourth year Ph.D. student advised by [Prof. Christopher
Ré](http://cs.stanford.edu/people/chrismre/) and affiliated with
the [DAWN](http://dawn.cs.stanford.edu), [SAIL](http://ai.stanford.edu), and [StatML](http://statsml.stanford.edu) groups. I am supported by the [Stanford Graduate Fellowship](https://vpge.stanford.edu/fellowships-funding/sgf/details) and the [National Science Foundation Graduate Research Fellowship](https://www.nsfgrfp.org).

My research interests revolve around _weak supervision_, or using high-level knowledge in the form of noisy labeling sources to efficiently label massive datasets required to train machine learning models. This includes systems like [Snorkel](https://github.com/HazyResearch/snorkel) and [Snorkel MeTaL](https://github.com/HazyResearch/metal) that allow users to write labeling functions rather than label data by hand. In this context, I'm also interested in using _developer exhaust_, byproducts of the data analytics pipeline, to simplify complex [statistical](#coral) and [search-based](#snuba) problems. 

<!-- My CV is [here](cv.pdf). -->

#### <a name="news"></a>Latest News

| 04/21/19 | Our paper on [Learning Dependency Structures for Weak Supervision Models](https://arxiv.org/pdf/1903.05844.pdf) accepted to ICML 2019!

| 04/10/19 | Our workshop paper on [Utilizing Weak Supervision to Infer Complex Objects and Situations in Autonomous Driving Data]() accepted to IEEE Intelligent Vehicles Symposium 2019!

| 03/22/19| Lab members use Snorkel MeTaL to [achieve state-of-the-art](https://dawn.cs.stanford.edu/2019/03/22/glue/) performance on the [GLUE Benchmark](https://gluebenchmark.com/leaderboard)

| 10/15/18 | [Snuba: Automating Weak Supervision to Label Training Data](http://www.vldb.org/pvldb/vol12/p223-varma.pdf) accepted to VLDB 2019!

#### <a name="project"></a>Projects

##### <a name="deps"></a>Learning Dependency Structures for Weak Supervision Models
###### ICML 2019
[Fres Sala](https://stanford.edu/~fredsala/) and I use a robust PCA-based algorithm to learn dependency structures among weak supervision sources without using any labeled data. We take advantage of the sparsity pattern in th structure and improve the sample complexity of existing efforts. We provide an information-theoretic lower bound on the minimum sample complexity of the weak supervision setting and empirically show that it improves over existing methods in terms of the quality of training labels generated. [[pdf](https://arxiv.org/pdf/1903.05844.pdf)] [[code](https://github.com/HazyResearch/metal)]

##### <a name="snuba"></a>Snuba: Automating Weak Supervision to Label Training Data
###### VLDB 2019
We explore how we can make weak supervision techniques easier to adopt by automating the process of generating noisy labeling heuristics. 
We introduce a system that takes as input a small, labeled dataset and a larger unlabeled dataset and assigns training labels to the latter automatically. It generates heuristics that each labels only the subset of the data it is accurate for, and iteratively repeats this process until the heuristics together label a large portion of the unlabeled data. We find that this method can outperform weak supervision with user-defined heuristics and crowdsourcing in many cases. [[pdf](http://www.vldb.org/pvldb/vol12/p223-varma.pdf)] [[code](https://www.github.com/HazyResearch/reef/)]

##### <a name="babble"></a>Babble Labble: Learning from Natural Language Explanations
###### ACL 2018, NeurIPS 2017 DEMO 
[Braden Hancock](https://www.bradenhancock.com/) and I explore how we can use natural language explanations for why crowd workers provide the labels they do to label training data more efficiently. We automatically parse these explanations into executable functions and apply them to large amounts of unlabeled data. We find that collecting explanations allows us to build high quality training sets much faster than collecting labels alone. [[pdf](https://arxiv.org/abs/1805.03818)] [[code](https://github.com/HazyResearch/babble)] [[blogpost](https://hazyresearch.github.io/snorkel/blog/babble_labble.html)] [[demo video](https://www.youtube.com/watch?v=YBeAX-deMDg)]

##### <a name="deem"></a>Efficient Model Search using Log Data
###### DEEM @ SIGMOD 2018
We present preliminary methods that use the logs generated while training complex deep learning models to predict the performance of models with different architectures. We find that without training any new models, we can predict how well a model architecture will perform according to different metrics and within training time constraints. [[pdf](logsearch.pdf)]

##### <a name="coral"></a> Coral: Enriching Statistical Models with Static Analysis
###### NeurIPS 2017, NeurIPS ML4H 2017, MED-NeurIPS 2017
We introduce a weak supervision framework to efficiently label image and video training data given a small set of user-defined heuristics. We identify correlations among heuristics using static analysis and incorporate this information into a generative model that can optimally assign probabilistic labels to training data. We apply this method to video querying and medical image classification tasks, outperforming fully supervised models in some cases. 
[[pdf](https://papers.nips.cc/paper/6628-inferring-generative-model-structure-with-static-analysis.pdf)] [[blogpost](http://dawn.cs.stanford.edu/2017/09/14/coral/)] [[video](https://youtu.be/Do1On5AzHE4)]

##### <a name="socratic"></a>Socratic Learning: Finding Latent Subsets in Training Data
###### HILDA @ SIGMOD 2017, NeurIPS FILM 2016
We explore how we can find latent subsets in training data that affect the behavior of weak supervision sources. We automatically identify these subsets using disagreements between the discriminative and generative models and correct misspecified generative models accordingly. We improve upon existing relation extraction and sentiment analysis tasks and make these latent subsets interpretable for users. 
[[pdf](https://arxiv.org/abs/1610.08123)] [[workshop](flipper.pdf)] [[blogpost](http://hazyresearch.github.io/snorkel/blog/socratic_learning.html)] [[video](https://www.youtube.com/watch?v=0gRNochbK9c)] 


#### <a name="pubs"></a>Publications
##### 2018
[Snuba: Automating Weak Supervision to Label Training Data](http://www.vldb.org/pvldb/vol12/p223-varma.pdf)  
**Paroma Varma** and Christopher Ré.  
To appear at *International Conference on Very Large Databases (VLDB), 2019*

[Weakly supervised classification of rare aortic valve malformations using unlabeled cardiac MRI sequences](https://nature-research-under-consideration.nature.com/users/37265-nature-communications/posts/38921-weakly-supervised-classification-of-rare-aortic-valve-malformations-using-unlabeled-cardiac-mri-sequences)  
Jason Fries, **Paroma Varma**, Vincent Chen, Ke Xiao, Heliodoro Tejeda, Saha Priyanka, Jared Dunnmon, Henry Chubb, Shiraz Maskatia, Madalina Fiterau, Scott Delp, Euan Ashley, Christopher Ré and James Priest.

[Training Classifiers with Natural Language Explanations](https://arxiv.org/abs/1805.03818)  
Braden Hancock, **Paroma Varma**, Stephanie Wang, Percy Liang and Christopher Ré.  
In *Association for Computational Linguistics (ACL), 2018*

[Exploring the Utility of Developer Exhaust](logsearch.pdf)  
Jian Zhang, Max Lam, Stephanie Wang, **Paroma Varma**, Luigi Nardi, Kunle Olukotun and Christopher Ré.  
In *Workshop on Data Management for End-to-End Machine Learning (DEEM) at SIGMOD, 2018*

##### 2017
[Inferring Generative Model Structure with Static Analysis](https://papers.nips.cc/paper/6628-inferring-generative-model-structure-with-static-analysis.pdf)  
**Paroma Varma**, Bryan He, Payal Bajaj, Imon Banerjee, Nishith Khandwala, Daniel L. Rubin and Christopher Ré.  
In *Neural Information Processing Systems (NeurIPS), 2017*

[Automated Training Set Generation for Aortic Valve Classification]()  
Vincent Chen, **Paroma Varma**, Madalina Fiterau, James Priest  and Christopher Ré.  
In *Machine Learning for Health (ML4H), Neural Information Processing Systems (NeurIPS), 2017*

[Generating Training Labels for Cardiac Phase-Contrast MRI Images]()  
Vincent Chen, **Paroma Varma**, Madalina Fiterau, James Priest  and Christopher Ré.  
In *Medical Imaging meets NeurIPS (MED-NeurIPS), 2017*

[Augmenting Generative Models to Incorporate Latent Subsets in Training Data](https://arxiv.org/abs/1610.08123)  
**Paroma Varma**, Bryan He, Dan Iter, Peng Xu, Rose Yu, Christopher De Sa, Christopher Ré  

[Flipper: A Systematic Approach to Debugging Training Sets](flipper.pdf)  
**Paroma Varma**, Dan Iter, Christopher De Sa and Christopher Ré.  
In *Workshop on Human-In-the-Loop Data Analytics (HILDA) at SIGMOD, 2017*

##### 2016
[Socratic Learning](http://www.filmNeurIPS.com/wp-content/uploads/2016/11/FILM-NIPS2016_paper_9.pdf)  
**Paroma Varma**, Rose Yu, Dan Iter, Christopher De Sa, Christopher Ré  
In *Future of Interactive Learning Machines Workshop (FILM), Neural Information Processing Systems (NeurIPS), 2016*

[Efficient 3D Deconvolution Microscopy with Proximal Algorithms](https://www.osapublishing.org/abstract.cfm?uri=ISA-2016-JT3A.44)  
**Paroma Varma**, Gordon Wetzstein  
In *Computational Optical Sensing and Imaging, Imaging and Applied Optics, 2016*

[Nonlinear Optimization Algorithm for Partially Coherent Phase Retrieval and Source Recovery](http://ieeexplore.ieee.org/abstract/document/7476825/)  
Jingshan Zhong, Lei Tian, **Paroma Varma**, Laura Waller  
In *IEEE Transactions on Computational Imaging, 2016*

##### 2015
[Source Shape Estimation in Partially Coherent Phase Imaging with Defocused Intensity](https://www.osapublishing.org/abstract.cfm?uri=COSI-2015-CTh1E.5)  
Jingshan Zhong, **Paroma Varma**, Lei Tian, Laura Waller  
In *Computational Optical Sensing and Imaging, Imaging and Applied Optics, 2015*

[Design of a Domed LED Illuminator for High-Angle Computational Illumination](https://www.osapublishing.org/abstract.cfm?uri=isa-2015-ITh1A.2)  
Zachary Phillips, Gautam Gunjala, **Paroma Varma**, Jingshan Zhong, Laura Waller  
In *Imaging Systems and Applications, 2015*

#### <a name="past"></a>In the Past
Previously, I worked on problems related to computational imaging. As an undergraduate at UC Berkeley, I studied phase retrieval via partial coherence
illumination and digital holography in Prof. Laura Waller's [Computational Imaging
Lab](http://www.laurawaller.com/). I also rotated with Prof. Gordon Wetzstein’s [Computational Imaging
Group](http://www.computationalimaging.org) and looked at solving 3D
deconvolution problems more efficiently.

#### Teaching
At UC Berkeley, I was a teaching assistant for the first offering of [EE16A: Designing Information Devices and Systems](https://inst.eecs.berkeley.edu/~ee16a/) and helped develop course material for the class as well. I was also a teaching assistant for EE20: Structure and Interpretation of Signals and Systems. 







