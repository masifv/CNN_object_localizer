# CNN_object_localizer

Object localization with ResNet50 architecture. Uses pre-trained weights from imagenet (transfer learning).

Input is a color image. The network has two outputs, object class ([1, 0] for person and [0, 1] for background) and its bounding box coordinates (xmin, xmax, ymin, ymax). Class output (two neurons) uses binary cross-entropy (categorical loss) and bounding box output (4 neurons) uses L2 loss (regression loss). Total loss is a weighted sum of the losses and currently the weights are hand tuned. It is also possible to learn it.  

Trainng data for this code is from Pascal VOC challenge. You can download it by running wget http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar


