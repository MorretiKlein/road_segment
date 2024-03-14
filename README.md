# Segment road and lane road 

### multi-classes semantic segmentation
## Define folder

* `GGDataset`: dataset image.
* `models`: store model resnet_unet
* `model.ipynb`: create model.
* `main.ipynb`: result and test
## description 
- Dataset that I get from a competition about autonomous car Digital race 
- I use resnet as encoder for unet to segment road and lane road
- loss function : binary crossentropy + dice loss
- metrics: accuracy and dice coefficients 
## to run and check repository
- Have to create new environment and pip install tensorflow with cuda :
    1. conda create -n tensoflow_env python=3.10
    2. conda activate tensoflow_env
    3. conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
    4. python -m pip install "tensorflow==2.10"
    5. pip install opencv-python
    6. pip install matplotlib

## result:
* accuracy: 98% and dice coefficients 0.97 and FPS : 12
<img src="road.mp4" width="128"/>   <img src="road.mp4" width="400"/>

