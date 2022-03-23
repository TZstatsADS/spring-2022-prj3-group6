# Project: Weakly supervised learning-- label noise and correction

## Reproducibility 
The dataset is not available in this repo. Please download the dataset separately and then place it in the `data` folder, in it's own subfolder titled `images`. The labels are left for ease of use, but can be changed if the dataset or labels change. This project is a Python3 project, originally run in python 3.9 and 3.10. Ocassionally, Python will throw a naming issue on the first run of the Juypyter Notebook. Simply continue restart the run and it will resolve itself without any intervention.


### [Full Project Description](doc/project3_desc.md)


Term: Spring 2022

+ Team 06
+ Team members
	+ Noah Love
	+ Xiangyu Ma
	+ Peixuan Song - Built main model and visualization
	+ Vasiliki Vlachou
	+ Hahyung Jung - Reported COVID-19 Issue

+ Project summary: In this project, we created a successful image classifier that is capable of identifying and classifying images of 10 types: plane, car, bird, cat, deer, dog, frog, horse, ship and truck. 

### Feature Detector 
Our model involves stacking convolutional layers. Many of which are small 3x3 filters, with a LeakyReLU and then a max pooling layer. There are three of these, with increasing depth of the network from 32 to 128 for the first four blocks of the model. 

### Classifier Part
The classifier interprets the feature dectection and makes a prediction as to which class, in this case 1 of 10, the photo belongs. In our model, the feature extraction is flattened, using a variety of activations, down to 10 nodes for 10 classes. 

### Capabilities
This model improves significantly on the baseline model, and model II improves greatly over model I. We strongly recommend implementing model I in all use cases. It is capable of predicting images at a rate of *70%* accuracy, even with noisy labels.
	
	
**Contribution statement**: ([default](doc/a_note_on_contributions.md)) Hahyung Jung was unable to contribute to the project due to Covid. He has emailed the professor about this. Other team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
