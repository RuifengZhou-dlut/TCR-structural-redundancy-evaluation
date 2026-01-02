# TCR structural redundancy evaluation
These codes contains the experimental codes of Structural Redundancy Evaluation for Convolutional Neural Networks via Task Contribution Analysis. The codes runs on Tensorflow 2.7 and python 3.7.0, they also relies on pandas, scipy and libraries. The dataset used in this paper is CIFAR-10. 
# Introduction of TCR structural redundancy evalution 
As a method for evaluat structural redundancy, the TCR evaluation method is based on the CNN structured pruning algorithm and the linear probe method. By analyzing whether the channel outputs can have effective outputs that can assist the network in classification, it realizes the construction of quantitative criteria for the contribution of channels to the network. Based on this, a method for evaluating the redundancy of network substructures and a method for structuring pruning of the network are constructed to achieve the evaluation of structural redundancy of the entire network and its substructures.

Our evaluation method has the following advantages:

1) High intelligibility: This method ensures that the evaluation algorithm finds truly the redundant structures that have a relatively minor impact on the network in an intelligible manner.
   
2) Full objectivity: This evaluation method will try to eliminate the influence of subjective factors such as random factors and parameter settings as much as possible.
   
3) High applicability: The evaluation method can provide targeted evaluation results based on different tasks.
# Introduction to the evaluation algorithm code
The main part of the code is located in the class-3 and class-10 folders, while the plotting part is in the plot folder. The "class-3" folder contains the evaluation codes and results using the original training dataset and the distilled dataset, while the "class-10" folder only contains the evaluation codes and results using the distilled dataset. The evaluation results are all saved in.json files, while the evaluation code is in.ipynb files. The code consists of three types. The first type is data preparation code, usually including code related to data extraction and data distillation, and the names contain "data". The second category is the network training code. This code is used to train the network to be evaluated. It is named according to the network type, such as "VGG-16". The third category is for evaluating algorithm codes, and the names include "rude".
