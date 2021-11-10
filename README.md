# Social synchronization of conditioned fear in mice requires ventral hippocampus input to amygdala
Running title: Emotional synchronization in mice<BR>
Wataru Ito*, Alexei Morozov*

*This document describes the codes in the manuscript and how to run them using an example video, according to the nature portfolio, Reporting Summary, and Software and code.

# 1. Set up the Python environment
Conda and pip configured the Python environment. We describe here solely the installation on Windows 10 PC. The lines preceded by # are comment lines.

#### 1. Install Miniconda
Download the binary and install it as described on the web
https://docs.conda.io/en/latest/miniconda.html#windows-installers
    
#### 2. Open the Anaconda prompt and follow the sequence below.
```python
# anaconda, python 3.8 for MATLAB engine for python
conda update -n base -c defaults conda
conda create --name jl2
conda activate jl2
conda install python=3.8 anaconda
```
    
```python    
# matplotlib
# The following command request installation of node.js
# Download Nodo.js https://nodejs.org/en/download/<BR>
# Install https://github.com/nodejs/help/wiki/Installation
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install jupyter-matplotlib
jupyter nbextension list
```

```python 
# Install other packages
# for video process
pip install opencv-contrib-python
pip install ffmpeg-python
```

#### 3. Clone the GitHub code
Move to the folder you want to clone the GitHub code
```python
cd W:\wataru\jupyter\synchro_freeze
git clone https://github.com/frejanordsiek/hdf5storage.git
cd Codes_in_Emotional_sync_Ito_et_al
```
#### 4. Start Jupyter Lab.
```python
jupyter lab python_codes_in_manuscript.ipynb
```

#### 5. Set the root path
Set the current path as an absolute path.
