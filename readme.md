# Orthographic Feature Transform for Monocular 3D Object Detection

Note: Please use the dev branch for inference and training as the master branch(cloned from original repo) is incomplete. #

## Training
The training script can be run by calling `train.py` with the name of the experiment as a required position argument. 
```
python train.py name-of-experiment --gpu 0
```
By default data will be read from `data/kitti/objects` and model checkpoints will be saved to `experiments`. The model is trained using the KITTI 3D object detection benchmark which can be downloaded from [here](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d). See `train.py` for a full list of training options.

## Inference
To decode the network predictions and visualise the resulting bounding boxes, run the `infer.py` script with the path to the model checkpoint you wish to visualise:
```
python infer.py /path/to/checkpoint.pth.gz --gpu 0
```

