* Repository github url : https://github.com/jai-mr/
- Assignment Repository : https://github.com/jai-mr/Assignment-3
- Submitted by : Jaideep Rangnekar
- Registered email id : jaideepmr@gmail.com

## 1. Code_01_Final
- url : http://localhost:8888/notebooks/Documents/AI/Submission/S5/01.%20Code_01_Final.ipynb

* Target
Don't worry aboutthe params limit of <=10000 at this stage but get a good accuracy
Setup the basic training & Create a Baseline Model
Use of 15 Epochs
* Result
Params: 13,808
Best Train Accuracy: 99.21%
Best Test Accuracy : 99.27%
* Analysis
The model is not overfitting, but we need to reduce the number of params, since our target is 10K Params
Add data augmentation to possibly improve the model


## 2. 02_Code_02_Final
- url: https://github.com/jai-mr/Assignment-5/blob/master/02_Code_02_Final.ipynb

* Target
Reduce the number of parameters
Add Transformations
A -7deg to 7deg rotations should work for us
* Result
Params: 9,707
Best Train Accuracy: 98.88%
Best Test Accuracy : 99.27%
* Analysis
We added augmentation to compensate the removal of params but need to train the remaining neurons harder

## 3. 03_Code_03_Final
- url : https://github.com/jai-mr/Assignment-5/blob/master/03_Code_03_Final.ipynb

* Target
Add another layer after the GAP, possibly to capture more features
* Result
Params: 9,707
Best Train Accuracy: 98.12%
Best Test Accuracy : 99.14%
* Analysis
There was a marginal increase in the accuracy
We've reached our target parameters, but not the target accuracy
From the loss, accuracy plot we can see that there is a lot of oscillations, we could try to reduce this by using a LR Scheduler in the next iteration

## 4. 04_Code_04_Final
- url : https://github.com/jai-mr/Assignment-5/blob/master/04_Code_04_Final.ipynb

* Target
Add a LR Scheduler to reduce the oscillations
* Result
Params: 9,962
Best Train Accuracy: 98.26%
Best Test Accuracy : 99.26%
* Analysis
There is a increase in accuracy conveying that LR is working

## 5. 05_Code_05_Final
- url : https://github.com/jai-mr/Assignment-5/blob/master/05_Code_05_Final.ipynb

* Target
Fine Tune the Transforms, set rotation to -10deg to 10deg
Use the OneCycleLR Scheduler since the PyTorch Documentation says The 1cycle learning rate policy changes the learning rate after every batch. step should be called after a batch has been used for training.
*  Result
Params: 9,962
With
Best Train Accuracy: 98.11%
Best Test Accuracy : 99.33%
* Analysis
Now the learning is consistent, the accuracy increases

