# Social synchronization of conditioned fear in mice requires ventral hippocampus input to amygdala
Running title: Emotional synchronization in mice<BR>
Wataru Ito*, Alexei Morozov*

*This document describes the codes in the manuscript and how to run them using an example video.
    
# Set up the Python environment
Conda and pip configured the Python environment. We describe here installation only on Windows 10 PC. The lines preceded by # are comment lines. The installation procedure was tested on 11/10/2021 using a freshly installed Win10 PC.

#### 1. Install Windows apps
1. Miniconda<BR>
Download the binary and install it as described on the web<BR>
https://docs.conda.io/en/latest/miniconda.html#windows-installers
2. node.js<BR>
Download Nodo.js from https://nodejs.org/en/download/
3. ffmpeg<BR>
    a) Download ffmpeg-git-full.7z from https://www.gyan.dev/ffmpeg/builds/<BR>
    b) Move the folder `ffmpeg-2021-11-07-git-45dc668aea-full_build` to `C:\Program Files`.<BR>
    (The folder name might be different depending the timing of download.)<BR>
    c) Set the system path.<BR>
    Click `Windows Start button` and type "env". Click the `Edit the system environment variables`.<BR>
    
    <img src="img/Screenshot 2021-11-10 170410.png" width=200px><BR>
    
    Click `Environment Variables...`.<BR>
    
    <img src="img/Screenshot 2021-11-10 170711.png" width=300px><BR>
    
    Select "Path" in the lower "System variables" panel and Click `Edit...`<BR>

    <img src="img/Screenshot 2021-11-10 171038.png" width=300px><BR>
    
    Click `New` and enter the path as shown below.<BR>
    
    <img src="img/Screenshot 2021-11-10 141544.png" width=300px><BR>   
    
#### 2. Open the Anaconda prompt and follow the sequence below.
1. In the Anaconda prompt

```python
# anaconda, python 3.8 for MATLAB engine for python
conda update -n base -c defaults conda
conda create --name jl2
conda activate jl2
conda install python=3.8 anaconda
```

```python
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install jupyter-matplotlib
jupyter nbextension list
```

```python 
# Install other packages for video process
pip install opencv-contrib-python
pip install ffmpeg-python
```

#### 3. Download the codes and start Jupyter Lab
1. Go to https://github.com/wataruito/Codes_in_Emotional_sync_Ito_et_al
2. Select the "Code/Download ZIP"<BR>
    
<img src="img/Screenshot 2021-11-10 145736.png" width=400px><BR>
    
3. Extract the downloaded zip file.
4. Place the `Codes_in_Emotional_sync_Ito_et_al-main` folder to an appropriate place.


#### 4. In the opened the Anaconda prompt   
1. Change the current directory into the `Codes_in_Emotional_sync_Ito_et_al-main` folder.
2. Start Jupyter Lab.
    
```python
jupyter lab python_codes_in_manuscript.ipynb
```
    
Follow "1. Set the root path" in the opened notebook.
