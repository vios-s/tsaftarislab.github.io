---
title: "DREAM: Disentangled Representations for Efficient Algorithms for Medical data"

collection: tutorials
permalink: /tutorials/dream2020
sidebar:
  nav: "dream"
---
A MICCAI 2020 (Peru) Tutorial by Sotirios A. Tsaftaris and Alison Q. O'Neil.

![DREAM 2020]({{ base_path }}/assets/images/dream.png)

## Outline {#outline}
Disentangled representation learning has been proposed as an approach to
learning general representations. This can be done in the absence of
annotations, or with limited annotation. A good general representation can be
readily fine-tuned for new target tasks using modest amounts of data. This
alleviation of the data and annotation requirements offers tantalising prospects
for tractable and affordable healthcare. Finally, disentangled representations
can offer model explainability, increasing their suitability for real-world
deployment. In this half-day tutorial we will offer an overview of
representation learning and disentangled representation learning and criteria,
and discuss applications in medical imaging. We will conclude with open ended
challenges. 

## Program {#program}
1. Part 1: 30mins
  * Representation learning
  * Compositionality theory
  * Invariance and covariance and the information bottleneck principle
2. Part 2: 1hr
  * Disentangled learning
  * VAE and GANs and disentangling variants
  * Metrics for disentanglement
3. Coffee break (20mins)
4. Part 3: 1hr
  * Content-style disentanglement
  * The complexities of multimodal and multitask learning
5. Part 4: 1hr
  * Applications of disentanglement in medical imaging, computer vision and healthcare
  * Open challenges and Q&A

## Learning Objectives {#objectives}
* Understand representation space and why (in)variance matters
* Understand the theories of information bottleneck and compositionality
* Learn the different objectives in achieving disentanglement
* Appreciate the inductive biases introduced by network design choices
* Appreciate when disentanglement is useful in practice

## Motivation {#motivation}
Imagine that we want to develop a system that localises the heart in MRI and CT
images. This system will need to be robust to any changes in imaging, the
scanner, noise, and critically anatomical and pathological variation. The
current paradigm with deep learning is that we *must* present to the system as
many examples as possible to make it robust and learn what is nuisance (e.g.
noise and imaging differences) as opposed to what matters (e.g. the location of
the heart). [A similar argument can be made for organs in a CAI setting.]

Clearly this is not sustainable and leads to poor performance.
Disentangled learning can help because it allows us to learn latent factors that
can describe what we see in the data. In the example on the right, we can
imagine a latent factor that one learns a change in pose (or in the patient for
the cardiac example), and another factor for the change in a car's colour (or a
different scanner). Surprisingly we do not always need annotated data to achieve
this. Moreover, it has been shown that disentangled representations are privacy
preserving; can offer explainability and interpretability; and can generalise to
new tasks (meta-learning) and to new data sources with less effort.

We should (re)appreciate that machine learning (ML) is not simply a functional
mapping between input and output, but one that maps input data to manifolds and
then decisions/tasks. This return to principled design will allow us to evolve
and propose efficient solutions that are robust to new applications and shorten
the path to clinical translation.

Learning suitable representations is key in ML. In fact, the ML community has
the dedicated International Conference on Learning Representations
([ICLR](https://iclr.cc/)). Disentangled learning is considered a hot area: a
dedicated [challenge run at NeurIPS
2019](https://www.aicrowd.com/challenges/neurips-2019-disentanglement-challenge).
According to Google Scholar trends, the number of papers in major ML conferences
doubles yearly . Scientific American, a prestigious periodical in popular
science, had a description of disentangled representation learning in May 2019
([Machine Learning Gets a Bit More
Humanlike](https://www.scientificamerican.com/article/machine-learning-gets-a-bit-more-humanlike/)).
Disentangled learning appeared in MICCAI 3 years ago in a couple of papers, but
now has tripled in appearance. Thus, it is timely to formally introduce this
important area of research in our community.

## Teachers {#teachers}
Prof. Sotirios A. Tsaftaris (Sotos) is Chair in Machine Learning and Computer
Vision with the University of Edinburgh and is also the Canon Medical/Royal
Academy of Engineering Research Chair in Healthcare AI. Sotos leads a group
where several young researchers work in machine learning and computer vision. He
obtained his PhD in 2006 from Northwestern University USA and has held several
academic positions in USA, Italy and UK. Sotos's research expertise is in
representation learning. 

Dr Alison Q. O'Neil (Alison) is a Senior Scientist in the AI Research Team at
Canon Medical Research Europe and Honorary Research Fellow at the University of
Edinburgh. She obtained her EngD at Canon Medical Research Europe in affiliation
with Heriot-Watt University, and now leads a team of scientists and research
students working on machine learning techniques for industrial healthcare
applications – including applications in medical imaging, natural language
processing, and electronic health record (EHR) data. Alison will bring an
industry perspective to the tutorial and also talk about disentanglement in
other data forms (e.g. text). 

## Materials {#materials}
Slides, notes and accompanying list of references (forthcoming).

## Support {#support}
Generously supported by [Canon Medical Research
Europe](https://research.eu.medical.canon/), the [Royal Academy of
Engineering](https://www.raeng.org.uk/) and the
[School of Engineering](https://www.eng.ed.ac.uk/).  
