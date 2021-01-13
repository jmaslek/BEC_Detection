# BEC_Detection

The goal here is to extract a ROI from an experimentally obtained image that may contain 1-9 BEC (or thermal) clouds.  This allows for a speedup in computations involving peak fitting to extract numerical parameters (such as widths/positions/atom number).

This uses the Matterport Mask_RCNN algorithm.  Training data are hand labeled using the online VGG annotator.  Training is done in Google Colab using the GPU runtime.  The detection seems to converge pretty quickly, as 20 epochs was enough.

The one downside to this is that I used the training data as the validation data, which is bad practice, but given the annotations that I actually had (only about 100), I decided to use them all for training.

