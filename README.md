# AI_Algorithm-1
## Installation
First, navigate a terminal to the AI_Algorithm directory and run `pip install pipenv`
Then, run `pipenv --python path/to/64-bit/python.exe install` where `path/to/64-bit/python.exe` is the path to a 64 bit python installation on your machine. If the only python installation you have is 64 bit, the you can just run `pipenv install`.
If you get an error installing tensorflow, it is likely you are not using a 64 bit python.
Next, run `pipenv shell` and then `python -m pip install -U ./models/research` . Then run `pip install numpy==1.17` and ignore the error. You should now be able to run `python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=wally_model_v6/pipeline.config --checkpoint_dir=wally_model_v6` to test the model on the training data and `python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=exported_models/wally_model_v6/pipeline.config --checkpoint_dir=wally_model_v6` to test the model on the training data. 
If this fails, go to the [TensorFlow Object Detection API Documentation](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html) and [Pytorch Documentation](https://pytorch.org/get-started/locally/) and follow the installation instructions there.

# Where's Waldo AI 
This program runs the Object Detection code to find Waldo from 10 images. 

## Contributors: Team 5
Adam Sickels, Kayla Manouchehri, Abha Naik, Sery Gunawardena, Chase Fensore

## Table of Contents:
- Repository Setup
- Gem Installations
- Classes
- Program Instructions 
- Testing

## Repository Setup:

Clone repository by running 'git clone https://github.com/kaymano/AI_Algorithm-1' in terminal

## Requirements
- 64-bit python installation between 3.6 and 3.9, but not including 3.9
- pip
- (Microsoft C++ Build Tools)[https://visualstudio.microsoft.com/visual-cpp-build-tools/]

## Installations:
1. Navigate to the AI_Algorithm-1 directory

2. Install pipenv
```bash
pip install pipenv
```
3. If you do not have 64-bit python or are running python 3.9, run
```bash
pipenv --python path/to/64-bit/python.exe install
```
where path/to/64-bit/python.exe is a path to a 64 bit installation of python between version 3 and 3.9

Otherwise, run
```bash
pipenv install
```
4. 
```bash
pipenv shell
```

5. 
```bash
python -m pip install -U ./models/research
```

6. 
Install numpy and if there is an error, ignore it. 
```bash
pip install numpy==1.17
```

## Program Instructions

Test the model on training images
```bash
python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=wally_model_v6/pipeline.config --checkpoint_dir=wally_model_v6
```

Test the model on testing images
```bash
python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=wally_model_v6/pipeline_test.config --checkpoint_dir=wally_model_v6
```

After running these commands and the mAP appears, you can press ^C to terminate the program
First, run `pip install pipenv`
Then, run `pipenv --python path/to/64-bit/python.exe install` where `path/to/64-bit/python.exe` is the path to a 64 bit python installation on your machine. If the only python installation you have is 64 bit, the you can just run `pipenv install`.
If you get an error installing tensorflow, it is likely you are not using a 64 bit python.
Next, run `pipenv shell` and then `python -m pip install -U ./models/research` . Then run `pip install numpy==1.17` and ignore the error. You should now be able to run `python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=wally_model_v6/pipeline.config --checkpoint_dir=wally_model_v6` to test the model on the training data and `python models/research/object_detection/model_main_tf2.py --model_dir=wally_model_v6 --pipeline_config_path=wally_model_v6/pipeline_test.config --checkpoint_dir=wally_model_v6` to test the model on the testing data. 
If this fails, go to the [TensorFlow Object Detection API Documentation](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html) and [Pytorch Documentation](https://pytorch.org/get-started/locally/) and follow the installation instructions there.


