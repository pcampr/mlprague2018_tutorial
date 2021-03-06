# Deep Learning for Music Classification using Keras

(c) 2018 by

**Alexander Schindler**, AIT Austrian Institute of Technology<br>
http://ifs.tuwien.ac.at/~schindler

**Thomas Lidy**, Musimap<br>
http://ifs.tuwien.ac.at/~lidy

# Abstract

Deep Learning has re-entered the field of Machine Learning with a big bang. Tasks that were difficult and cumbersome to solve are now simple to implement and achieve amazingly high accuracies. Deep Learning has shown substantial impact recently also in the domain of audio recognition and music classification. This tutorial will give a general introduction to Neural Networks, Convolutional Neural Networks, plus important concepts such as (batch-)normalization, training epochs, activation, loss, optimization, pooling, dropout, model fine-tuning, etc. and a tutorial on how to apply all of this on tasks of audio and music recognition using the convenient Python Keras framework on top of Tensorflow. It will use T-SNE for visualization and also cover unsupervised learning.

# Code and Data Availability

Dear workshop participants. The code and data for this workshop will be made available for download on Wednesday, March 21, 2018.

# Tutorial Requiremnets

For the tutorials, we use iPython / Jupyter notebook, which allows to program and execute Python code interactively in the browser.

### Viewing Only

If you do not want to install anything, you can simply view the tutorials' content in your browser, by clicking on the tutorial's filenames listed below in the GIT file listing (above, resp. on https://github.com/... ).

The tutorial will open in your browser for viewing.

### Interactive Coding

If you want to follow the Tutorials by actually executing the code on your computer, please [install first the pre-requisites](#installation-of-pre-requisites) as described below.

After that, to run the tutorials go into the `mlprague2018_tutorial` folder and start from the command line:

`jupyter notebook`


# Installation of Pre-requisites

## Install Python 2.7

Note: On most Mac and Linux systems Python is already pre-installed. Check with `python --version` on the command line whether you have Python 2.7.x installed.

Otherwise install Python 2.7 from https://www.python.org/download/releases/2.7/

## Install Python libraries:

### Mac, Linux or Windows

(on Windows leave out `sudo`)

```
sudo pip install jupyter
```

Try if you can open 
```
jupyter notebook
```
on the command line. 

Then download or clone the Tutorials from this GIT repository:

```
git clone https://github.com/slychief/mlprague2018_tutorial.git
```
or download https://github.com/slychief/mlprague2018_tutorial/archive/master.zip <br/>
unzip it and rename the folder to `mlprague2018_tutorial`.

Install the remaining Python libraries needed:

Either by:

```
sudo pip install Keras==2.1.5 Tensorflow scikit-learn pandas librosa
```

or, if you downloaded or cloned this repository, by:

```
cd mlprague2018_tutorial
sudo pip install -r requirements.txt
```

### Optional for GPU computation

If you want to train your neural networks on your GPU, also install the following (not needed for the tutorials):

* [NVidia drivers](http://www.nvidia.com/Download/index.aspx?lang=en-us)
* [CUDA](https://developer.nvidia.com/cuda-downloads)
* [cuDNN](https://developer.nvidia.com/cudnn) (optional, for further speedup)

# Source Credits

## Python libraries

The following helper Python libraries are used in these tutorials:

* `image_preprocessing.py`: by Thomas Lidy and Alexander Schindler
* `audiofile_read.py` and `rp_extract.py`: by Thomas Lidy and Alexander Schindler, taken from the [RP_extract](https://github.com/tuwien-musicir/rp_extract) git repository
* `wavio.py`: by Warren Weckesser

## Data Sources

The data sets we use in the tutorials are from the following sources: (a copy is included in this repository, so no need to download them)

* Music Speech Data Set:
by George Tzanetakis
Collected for the purposes of music/speech discrimination. Consists of 128 tracks, each 30 seconds long. Each class (music/speech) has 64 examples in 22050Hz Mono 16-bit WAV audio format.
http://marsyasweb.appspot.com/download/data_sets/

### Prepared Datasets for Download

**MagnaTagAtune**

https://owncloud.tuwien.ac.at/index.php/s/hivOGXKoUQtacbo (332MB)


**GTZAN Music Speech Classification**

https://owncloud.tuwien.ac.at/index.php/s/JiBXUPZK9LImTHB (145MB)

