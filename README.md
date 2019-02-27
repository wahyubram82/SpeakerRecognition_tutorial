# SpeakerRecognition_tutorial

A pytorch implementation of d-vector based speaker recognition system.  
All the features for training and testing are uploaded. 

## Requirements
python 3.5+  
pytorch 1.0.0  
pandas 0.23.4  
numpy 1.13.3  
pickle 4.0  
matplotlib 2.1.0  

## Datasets
We used the dataset collected through the following task.
- No. 10063424, 'development of distant speech recognition and multi-task dialog processing technologies for in-door conversational robots'

Specification
- Korean read speech corpus (ETRI read speech)
- Clean speech at a distance of 1m and a direction of 0 degrees
- 16kHz, 16bits  

We uploaded log mel filterbank energy features extracted from the above dataset.  
[python_speech_features](https://github.com/jameslyons/python_speech_features) library is used.

### * Train
24000 utterances, 240 folders (240 speakers)  
Size : 3GB  
```feat_logfbank_nfilt40 - train```

### * Enroll & test
20 utterances, 10 folders (10 speakers)  
Size : 11MB  
```feat_logfbank_nfilt40 - test```

## Usage
### 1. Training
```python train.py```  

### 2. Enrollment
```python enroll.py```  

### 3. Testing
For speaker verification,  
```python verification.py```  

For speaker identification,  
```python identification.py```



## Author
Youngmoon Jung (dudans@kaist.ac.kr) at KAIST, South Korea
