# NaiveBees

This repository provides the winning solution to DrivenData's NaiveBees competition.

## Create training file list 

    python create_training_dataset.py 


## Run caffe 

put bvlc_googlenet.caffemodel in ./ 

Run:

    ./PATH_TO_CAFFE/caffe train ­solver ./solver.prototxt ­weights ./bvlc_googlenet.caffemodel 

snapshots are saved every 1000 iterations to ./snapshots/ 
 
Caffe must be run upto 20000 iterations. 
 
## Create test predictions 

    python create_preds.py 
 
##Make final predictions 
 
    python create_sub.py