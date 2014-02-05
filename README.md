## About TomoPy

TomoPy is a Python toolbox to perform data processing and image reconstruction 
tasks at [APS](http://www.aps.anl.gov/ "APS"). It uses
[HDF5 file format](https://github.com/data-exchange/data-exchange/ "Data Exchange")
as the standard means of data exchange.

## Clone the TomoPy project:
``$ cd to your working directory`` (i.e. /local/tomopy/)

``$ git clone https://github.com/tomopy/tomopy.git tomopy``

## External Dependencies:
- [HDF5 1.8.12](http://www.hdfgroup.org/HDF5/ "HDF5")
- [FFTW 3.3.3](http://www.fftw.org "FFTW3") (only float library is required)
- [Boost C++ 1.55.0](http://www.boost.org "Boost C++") (only thread, system and date_time libraries are required)

To automatically downaload and install the external dependencies inside ``/usr/local``:

``$ python install.py --fftw --boost`` 

or if authorization is required

``$ sudo python install.py --fftw --boost``

To install them to another directory use:

``$ python install.py <my-install-directory> --fftw --boost``

in case after the installation you should define ``LIB_TOMOPY`` as an environment variable: 

``$ setenv LIB_TOMOPY <your-path-to-libraries>`` 

before you start installing TomoPy.

## Python Dependencies:
- [NumPy 1.8.0](http://www.numpy.org "numpy")
- [SciPy 0.13.2](http://www.scipy.org "scipy")
- [H5Py 2.2.1](http://www.h5py.org "h5py")
- [PyWt 0.2.2](http://www.pybytes.com/pywavelets/ "pywt")
- [Pillow 2.3.0](https://pypi.python.org/pypi/Pillow// "pillow")

## Installing TomoPy

Make sure you have [Python 2.6](http://www.python.org/download/releases/2.6/ "tsss...") or [2.7](http://www.python.org/download/releases/2.7/ "tsss...") and the above dependencies installed in your system. If the external libraries are installed in a non-standard place, define the environment variable ``LIB_TOMOPY`` and set it to the location of the ``lib`` folder (like ``setenv LIB_TOMOPY <path-to-external-libraries>``). Then:

- To insall from an egg distribution download the [latest released egg](https://github.com/tomopy/tomopy/releases) for your system, open shell prompt and type `easy_install my-egg-name` in the directory where the egg resides.
- To build and install from source, download the tarball or clone the project, open shell prompt and type `python setup.py install` in the directory where `setup.py` resides.


