## Installation

The current CNN is implemented in Python v3.9 with Keras and Tensorflow 2, while the traffic pre-processing tool is implemented in Python v3.9, Numpy and Pyshark.

This model requires the installation of a number of Python tools and libraries. This can be done by using the ```conda``` software environment (https://docs.conda.io/projects/conda/en/latest/).
We suggest the installation of ```miniconda```, a light version of ```conda```. ```miniconda``` is available for MS Windows, MacOSX and Linux and can be installed by following the guidelines available at https://docs.conda.io/en/latest/miniconda.html#. 

For instance, in Linux OS, execute the following command and follows the on-screen instructions:

```
bash Miniconda3-latest-Linux-x86_64.sh
```

Similarly, in Mac OS:

```
bash Miniconda3-latest-MacOSX-arm64.sh
```

Then create a new ```conda``` environment (called ```python39```) based on Python 3.9:

```
conda create -n python39 python=3.9
```

Activate the new ```python39``` environment:

```
conda activate python39
```

Install Tensorflow 2.7.0. In a Linux OS:

```
(python39)$ pip3 install tensorflow==2.7.0 
```

On the new Apple's computers with M1 CPU, execute instead:

```
(python39)$ pip3 install tensorflow-macos==2.7.0 
(python39)$ pip3 install tensorflow-metal 
```

And finalise the installation with a few more packages:

```
(python39)$ pip3 install pyshark sklearn numpy tensorflow==2.7.0 h5py lxml
```



Pyshark is just Python wrapper for tshark, allowing python packet parsing using wireshark dissectors. This means that ```tshark``` must be also installed. On an Ubuntu-based OS, use the following command:

```
sudo apt install tshark
```

Please note that the current code works with ```tshark``` **version 3.2.13 or lower**. Issues have been reported when using newer releases such as 3.4.X.

For the sake of simplicity, we omit the command prompt ```(python39)$``` in the following example commands in this README.   ```(python39)$``` indicates that we are working inside the ```python39``` execution environment, which provides all the required libraries and tools. If the command prompt is not visible, re-activate the environment as explained above.




