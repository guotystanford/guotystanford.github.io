---
layout: archive
title: "Intelligent Acoustic Emission Monitoring"
collection: research
permalink: /research/Intelligent_AE/
---

## AE-PNet: A Deep-Learning P-Wave Arrival Picker for Laboratory Acoustic Emissions
<p align="justify">
Picking P-wave arrivals of AE waveforms is the first and foremost step in analyzing AE data at an advanced level such as event localization, conducting acoustic tomography and moment tensor inversion. Deep-learning P-wave arrival pickers have outperformed traditional non-machine-learning algorithms in seismology. However, determining the optimal training data set size for these models in laboratory settings has been lacking, which is important for the AE community with much less available manually picked AE data. Introducing <b>AE-PNet</b>, a deep-learning P-wave arrival picker, we investigated the minimum number of manually picked waveforms needed for effective AE-PNet training. This study revealed that <b>a minimum of 1500 manually picked waveforms is necessary for adequate AE-PNet generalization[1].</b> AE-PNet consistently outperformed the Akaike Information Criterion (AIC) picker, one of the most widely used traditional non-machine learning pickers, ultimately enhancing the accuracy and efficiency of AE data analysis。  
</p> 

<img src="/images/AEPNET.jpg"/>  
<h4 align="center">The architecture of AE-PNet.  
</h4>

<img src="/images/Input & output_AEPNET.jpg"/>  
<h4 align="center">The input (an AE waveform containing the P-wave arrival) and the output (the probability of P-wave arrival) of AE-PNet.  
</h4>

## Stanford Acoustic Emission Data set [(SAED)](https://purl.stanford.edu/mz374gr4108)
<p align="justify">
AI is transforming seismic data analysis, yet its application to lab-scale seismic counterparts, namely AE remains relatively underexplored. The primary challenge stems from the limited availability of labeled data—manually selected, picked, and weighted waveforms—within the AE community compared to the vast labeled datasets readily available in seismology. To this end, we created the Stanford Acoustic Emission Database (SAED) [2], which includes ~ 50,000 manually picked waveforms. To our knowledge, SAED is the largest open-labeled dataset in the AE field. Based on the SAED, we trained and tested AE-PNet, a deep-learning model designed to pick P-wave arrivals both accurately and efficiently.  
</p>

## AE waveform preprocessing platform
<p align="justify">
I have developed a AE waveform preprocessing platform incorporating the AE-PNet module. This platform have the functions of:
</p>

* Visulizing and checking AE waveforms;  
* Manually selecting AE events;  
* Automatically picking the arrival time and first peak of P-waves using AIC and AE-PNet picker
* Manually refining the automatic pickings
* Manually weighting the P-wave arrival pickings
<p align="justify">
This platform can facilitate creating labelled AE data for training deep-learning models in intelligent acoustic emission monitoring. 
</p> 

<img src="/images/Picking Platform_V1.jpg"/>  

<img src="/images/Picking Platform_V2.jpg"/> 
<h4 align="center">AE P-wave arrival picking platform incorporating the AE-PNet module  
</h4>

<iframe width="300" src="https://www.youtube.com/embed/4AATCIqyOFU" title="YouTube video player" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Reference:
\[1\] <b>Guo T.Y.\*</b>, Vanorio T., & Ding J. (2024). A Deep-learning P-wave Arrival Picker for Laboratory Acoustic Emissions: Model Training and its Performance. <i>Rock Mechanics and Rock Engineering</i>. 1-19. [https://doi.org/10.1007/s00603-024-04296-5](https://doi.org/10.1007/s00603-024-04296-5)  
\[2\] <b>Guo T.Y.\*</b>, Vanorio T., & Ding J. (2024). Stanford Acoustic Emission Data set. <i>Stanford Digital Repository</i> [https://purl.stanford.edu/mz374gr4108](https://purl.stanford.edu/mz374gr4108)  