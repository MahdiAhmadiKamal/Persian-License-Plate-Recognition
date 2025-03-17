# Persian License Plate Recognition 🔎🚘🚔🚖


<img src="pics\img3.jpg" width="600">
<img src="pics\img4.jpg" width="600">

The initial part of this project involves using [deep-text-recognition-benchmark](https://github.com/clovaai/deep-text-recognition-benchmark) repository. First, the demo part is run, showing the capabilities of this repository. Then, it is examined whether English and Persian hand-writing text images and license plate images can be recognized correctly or not.

<img src="pics\img1.png" width="600">
<img src="pics\img2.png" width="700">

In the second and main part of this project, **Persian License Plate Recognition** is carried out with the aid of deep-text-recognition-benchmark. For this purpose, a [pretrained model](https://drive.google.com/drive/folders/15WPsuPJDCzhp2SvYZLRj8mAlT3zmoAMW) is selected and fine-tuned on a Persian license plates dataset called [IR-LPR](https://github.com/mut-deep/IR-LPR?tab=readme-ov-file). The data are labeled according to the following table.

<img src="pics\img5.png" width="800">

## Results

The results of the trained model are listed below.

| Iteration	| Train loss | Validation loss | Best accuracy |
| --------------- | --------------- | --------------- | --------------- |
| 4500 | 0.024 | 0.520 | 80.320 |

<table>
  <tr>
    <td>Input image</td>
    <td><img src="Persian_License_Plate_Recognition\test_images\16C32712.jpg" width="120"></td>
    <td><img src="Persian_License_Plate_Recognition\test_images\21W61612.jpg" width="120"></td>
    <td><img src="Persian_License_Plate_Recognition\test_images\27A46412.jpg" width="120"></td>
    <td><img src="Persian_License_Plate_Recognition\test_images\37R51160.jpg" width="120"></td>
    <td><img src="Persian_License_Plate_Recognition\test_images\66T41212.jpg" width="120"></td>
  </tr>
  <tr>
    <td>Predicted label</td>
    <td>16c32712 (c=س)</td>
    <td>21w61612 (w=د)</td>
    <td>27a46218 (a=الف)</td>
    <td>37r5116 (r=ط)</td>
    <td>66t41212 (t=ت)</td>
  </tr>
   <td>Confidence score</td>
    <td>0.9959</td>
    <td>0.9975</td>
    <td>0.0376</td>
    <td>0.9973</td>
    <td>0.9962</td>
  </tr>
</table>



## How to Install
Run following command:
```
pip install -r requirements.txt
```

## Usage

To create your own dataset, run:
```
Persian_License_Plate_Recognition\my_dataset_creation\plp_detection.ipynb
```
For license plate recognition using your own dataset, follow the instructions in [deep-text-recognition-benchmark](https://github.com/clovaai/deep-text-recognition-benchmark?tab=readme-ov-file) and run:
```
Persian-License-Plate-Recognition\Persian_License_Plate_Recognition\plp_recognition.ipynb
```


## Python
This project is accomplished using [Python](https://www.python.org/) language and the following tools:

<img src="pics/opencv.webp" width="170">
<img src="pics/matplotlib.png" width="170">
<img src="pics/yolov8.png" width="170">