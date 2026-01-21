In this project we address the problem of human pose estimation from still images through the implementation of a simple pipeline. Starting from raw RGB images of the LSP Dataset, our code predicts the 2D location of human body keypoints and evaluates their accuracy using standard pose estimation metrics (PCJ and PCP).

Once the pose estimation stage is completed, the predicted joint coordinates are used as the basis for an action recognition task. Since the LSP dataset does not provide action annotations, we first generate pseudo-labels by applying K-means clustering to these features.

Using the same pose-derived features, we then train and evaluate several classifiers, including neural models (MLPs) and classical machine learning method such as Random Forests. In addition, we also test the same classification pipeline using a set of manually annotated action labels.
