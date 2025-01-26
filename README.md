# SWIN_Transformer_optimisation
The mini project was aimed at the optimisation of a MASK RCNN model with a SWIN Transformer backbone. 
A total of two notebooks have been added to the repository. 
The first notebook: `FInal_Submission.ipynb` is where the task of `Pruning`, `Low Rank Transformation` and `Quantization` has been performed on a model, while on the other hand the second notebook: `Weight_clustering.ipynb` involves a small POC for `weight clustering`.


**Prereqisites** :
MMdetection and all its necessary dependencies must be setup. The notebook files already have a section under `Setup` with the help of which one can perform the same on google collab. In order to have a local setup, one must follow the official documentation of MMDetection. More information can be obtained at the following url:
[MMDetection](https://mmdetection.readthedocs.io/en/latest/get_started.html#)

**Tasks Covered**: 
The repository covers files that perform optimisations on the SWIN transformer. Overall , the optimisations can be performed on any model. However, the tasks must be tweeked according to the underlying downstream task. 

Here, I have covered: 
Pruning (as given by Pytorch) : [Pytorch Pruning](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html),
Quantisation(as given by Pytorch) : [Pytorch Quantisation](https://pytorch.org/docs/stable/quantization.html),
Low Rank Trasnformations

Similarly, a small 'Proof of Concept' was performed for the task of weight clustering. In order to actually achieve weight sharing using this involved digging deep into the mmdetection and mmcv libraries and change the way initialisation of weights takes place. We haven't covered the same in this scope.


