# Sklearn installation instruction on Ubuntu 16.04 LTS for Odroid XU4:

This is without anaconda. We do not have anaconda on the Odroid XU4.
Python version is 2.7. 

Official instructions are given in [Instructions link](http://scikit-learn.org/stable/install.html)
But the following instruction also have added options for a more elaborate installation, which is obtained after fixing some installation errors.

#### Install Dependencies for Sklearn:
```
sudo apt-get install python-numpy python-scipy python-matplotlib 
sudo apt-get install ipython ipython-notebook python-pandas python-sympy python-nose
```

#### Install Sklearn from Pip:
```
pip install -U scikit-learn
```

#### Install Dependencies for Skimage:
```
sudo apt-get install python-matplotlib python-numpy python-pil python-scipy build-essential cython
```

#### Clone the Skimage repository:

This is also from source. The official link for installation can be found [here](http://scikit-image.org/docs/dev/install.html).

```
git clone https://github.com/scikit-image/scikit-image.git
cd <skimage-directory>
pip install -e .
```

[ **NOTE:** do not forget the dot **'.'** in the end of this command ]

#### Run and Check:
Once the opencv has been installed, you can try to import it in a python script and see if it works properly.
To check if the opencv contrib modules are installed or not, you can try running the following statements in a python script.

```
python
>>> import sklearn, skimage
>>>
```
