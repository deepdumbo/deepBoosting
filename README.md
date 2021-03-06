Deep Boosting for Image Denoising
====
**Official implementation** for Deep Boosting Framework introduced in the following papers: <br/>
Chang Chen, Zhiwei Xiong, Xinmei Tian, Feng Wu. [Deep Boosting for Image Denoising](https://link.springer.com/content/pdf/10.1007%2F978-3-030-01252-6_1.pdf). In ECCV 2018. <br/>
Chang Chen, Zhiwei Xiong, Xinmei Tian, Zheng-Jun Zha, Feng Wu. [Real-world Image Denoising with Deep Boosting](https://ieeexplore.ieee.org/document/8733117). IEEE Transactions on Pattern Analysis and Machine Intelligence, in press. <br/>

## Requirements
Anaconda>=4.2.0 (Python 3.5) <br/>
TensorFlow==1.4.0 <br/>
Matlab Engine (Python Interface) <br/>

## Train the model
Usage example to train/evaluate a new model <br/>
```
cd train && cat train400.tfrecord.tar.gz.* | tar -xzv
python train.py && python inference.py
```

## Test the pre-trained models
Usage example to non-blind gray-level Gaussian image denoising <br/>
```
cd dn-nonblind-gray && python eval.py
```
Usage example to blind gray-level Gaussian image denoising <br/>
```
cd dn-blind-gray && python eval.py
```
Usage example to blind color Gaussian image denoising <br/>
```
cd dn-blind-color && python eval.py
```
Usage example to JPEG image deblocking <br/>
```
cd db-gray && python eval.py
```
Usage example to in-domain real-world image denoising <br/>
```
cd dn-real-in && python eval.py
```
Usage example to cross-domain real-world image denoising <br/>
```
cd dn-real-cross && python eval.py
```

## RID Dataset
To access Real-world Image Denoising (RID) dataset for training and validation <br/>
Download RID.tar.gz.0~5 from <br/>
[http://pan.bitahub.com/index.php?mod=shares&  
sid=eTJ2bFFQR3BzTm5FTGdjdXFBUnl2Y3htd3puWjFwRDc4SU9vSXc](http://pan.bitahub.com/index.php?mod=shares&sid=eTJ2bFFQR3BzTm5FTGdjdXFBUnl2Y3htd3puWjFwRDc4SU9vSXc)
```
cat RID.tar.gz.* | tar -xzv
```
To access Set60 benchmark for testing <br/>
```
cd datas/Set60
```
