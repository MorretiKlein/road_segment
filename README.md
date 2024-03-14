# Segment road and lane road 

### multi-classes semantic segmentation
## Define folder

* `GGDataset`: dataset image.
* `models`: store model resnet_unet.h5 and resnet_unet.h5.keras
"https://drive.google.com/drive/u/0/folders/1RM4TsMeZB22MbZiDui8RRAZRJ-ZeIJud"
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
7. pip install imageio
8. pip install imageio[ffmpeg]
## Result:
* Accuracy: 98%
* Dice Coefficients: 0.97
* FPS: 12

<img src="output_video.gif" />
