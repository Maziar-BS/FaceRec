# Face Recognition with Arcface

Real-time face recognition in unconstrained environments, based on [InsightFace](https://github.com/deepinsight/insightface). 

## Installation

install requirements
```
pip install -r requirements.txt
```

## Inference

For face detection, run the following command:
```
python inference_detection.py --input input/MBS.jpg
```

For face identification, feature extraction and comparisons, run the following command:
```
python inference_identification.py --input1 input/MBS0.jpg --input2 input/MBS1.jpg
```

For face recognition, run the following command:
```
python inference_recognition.py --input ./io/input/MBS2.jpg --update
```
The output will be saved in `./output` by default.

If you want to recognize your own faces, first thing you should do is to put your images at `./face_bank` directory and name them as in the followed structure:
```
face_bank
│
└───Person1_Name
│   │   Person1_Name_image_1.jpg
│   │   Person1_Name_image_2.jpg
│   │   ...
│   
└───Person2_Name
│   │   Person2_Name_image_1.jpg
│   │   Person2_Name_image_2.jpg
│   │   ...
│
│
...
```
Consequently, run the same commands as above with `--update` argument. Note that After each change in `./face_bank` directory, you should use `--update` argument again.
