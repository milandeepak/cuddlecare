# Cuddlecare Advanced Infant Monitoring System

## Description
Our project basically is a smart cradle that
- Rocks itself when the baby starts crying and ceases when the crying subsides
- Transmits the temperature and humidity around the cradle to a website

## Tech used
- Tensorflow lite model for cry detection
  	- It detects just background noise and cry
- Mediapipe
 	- MediaPipe is a framework for building on-device machine learning (ML) applications, offering low-code APIs, no-code studio, and flexible pipelines. It supports mobile (Android, iOS), web, desktop, edge devices, and IoT.
- Tkinter for visualising graphical interface

## How to run
First install the requirements.txt file
```py		
  pip install requirements.txt 
```
Then the format is 
```
 python classify.py --model modelname --overlappingFactor 0.75
```
so in our case 
```
python classify.py --model baby.tflite --overlappingFactor 0.75
```
## Demo
1. Demo of the graphical interface where the cry detection takes place
![Demo](https://github.com/milandeepak/cuddlecare/blob/076e2c1b8c53b9c5891aa0c18bcf57a6bdc52e2b/demo.gif)

2. Demo of the graphical interface and the motor that will rock the cradle

https://github.com/milandeepak/cuddlecare/assets/71485068/34edbee6-0de6-4670-8133-c6fcb6d84199

