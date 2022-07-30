# Machine-Learning-Neural-nets-Fine-grained-image-classification
# Fine-grained image classification | Using Birds Dataset| 200 categories of birds

This project uses the Caltech-UCSD Birds-200-2011 Dataset, found at:

http://www.vision.caltech.edu/visipedia/CUB-200-2011.html

Code Description
-----------------

- The code is contained in two .ipynb files, with annotations to help with understanding.

- This files are optimally opened in Colab so that Markdown annotations can be read.

- The cell outputs are included for convenience so that the code does not have to be run by you, as some of the models take many hours to complete.

-------------------------------------
1_Descriptive_Analysis
-------------------------------------

The first file is labelled `1_Descriptive_Analysis` and contains the code used to analyse the dataset.

The structure of the first file is as follows:

1. Relevant packages are imported.

2. Descriptive Analysis is conducted on the dataset. This takes ~1 hour to run.

-------------------------------------
2_Model_Implementation
-------------------------------------

The second file is labelled `2_Model_Implementation` and contains the code used to preprocess the dataset and train the models.

The structure of the second file is as follows:

1. Preprocessing of the dataset. This includes splitting the dataset into training and validation sets. This takes ~1 hour to run, with most of the time being taken to split the dataset.

2. Model implementation. 7 models are included in this code.
	Model 1 takes ~1.5 hours to run
	Model 2 takes ~3.5 hours to run
	Model 3 takes ~7 hours to run
	Model 3b takes ~7 hours to run
	Model 4 takes ~1 hour to run
	Model 5 takes <1 hour to run
	Model 6 takes <1 hour to run
		Since Models 3 and 3b take a long time to run, the results are saved for convenience of the user.

3. Results analysis of the models. This takes ~a few minutes to run.
	Written analysis is also briefly included here; see the report for more information.
  
# Conclusions
# Project Conclusions
The main conclusion of this project is the best model for use on CUB-200-2011. All the models performed 
well on the dataset, with the exception of LeNet. Despite being the most computationally expensive, 
EfficientNet performed the best overall, with high accuracies and loss values. DenseNet also performed 
fairly well and was one of the quickest models to run, which makes it a candidate. Overall, performance is 
valued over computation time, especially when considering that most fine-grain image classification models 
will be implemented on high-powered GPUs rather than Colab as was done in this project. As a result, 
EfficientNet is chosen as the best model for the CUB-200-2011 dataset, with DenseNet being presented as 
a cheaper, slightly lower-performance option.

# Suggestions for Future Work
The first suggestion for future work is to build a higher-quality database of images. There are many current 
databases available, but the quality of annotation and comprehensiveness of the categories could be 
improved. The performance of deep learning is positively correlated with the size of the database, so 
increasing their richness will improve performance and generalisation capabilities of future models.
Another area in which future models could improve is the effective use of local part information. A unique
feature of fine-grained image classification is that part features can be used to discriminate between 
classes. Using this part information is already a key part of research around this topic, and could be 
improved further in the future. This could be done through the use of these features, or the method of 
obtaining them. The first relies mainly on manual specification, which makes it difficult to generalise useful 
areas since they change across subcategories. The latter could be solved through more efficient partdetection algorithms. It should be noted that weakly-supervised fine-grained image classification is still a 
relatively new topic and will probably be the main direction of future research.
Lastly, the applications to real life are a key goal of fine-grained image classification: the practical 
application of models is the main value of their usefulness in this field. Current databases used in academic 
research tend to have prominent objects in the foreground for ease of training; the inclusion of more diverse 
image layouts would increase the generalisation of models in the future. For example, the CUB-200-2011 
database is mainly comprised of professional photographs of birds [1]; lighting, blur, occlusion, resolution 
and object interference should be more thoroughly represented. This could also be extended to finegrained video recognition, which is affected heavily by these factors.
  
