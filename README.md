# Caffe-to-CoreML-converter
A python script that converts Caffe trained model to CoreML in order to use natively with Swift CoreML

The project uses Oxford102.caffemodel as trained model. This model contains flowers and labels and give the ability to classify images and recognize the fauna.

As iOS only supports python v2.7, in order to run the scipt the following steps needs to be taken:

1. Download PIP for Python : https://pip.pypa.io/en/stable/installing/
2. Install PIP: 
```sudo python get-pip.py```
3. Install virtualEnv: 
```pip install virtualenv```
4. Create virtualEnv with python 2.7: 
```virtualenv --python=/usr/bin/python2.7 python27```
5. If step 4. fails, then install virtualEnv like this: 
```sudo /usr/bin/easy_install virtualenv```
6. Go into the environments folder where the environment was set up and run: 
```source python27/bin/activate```
7. If everything goes well, the prompt should show (python27). Now run: 
```pip install -U coremltools```
8. After installing coremltools, head to the folder and run the converter script: 
```python convert-script.py```
